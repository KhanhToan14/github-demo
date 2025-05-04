graph TD
    subgraph Thị trường
        P((Giá)) --- Q((Lượng))
        D[Đường cầu (D)]
        S[Đường cung (S)]
        E((Điểm cân bằng ($P_0, Q_0$)))
        Pc[Giá trần ($P_c < P_0$)]
        Qd[Lượng cầu tại $P_c$ ($Q^D$)]
        Qs[Lượng cung tại $P_c$ ($Q^S$)]
        ThieuHut[Thiếu hụt ($Q^D - Q^S$)]
        CS_truoc((Thặng dư tiêu dùng trước: 1 + 4))
        PS_truoc((Thặng dư sản xuất trước: 2 + 3 + 5))
        NB_truoc((Tổng lợi ích trước: 1 + 2 + 3 + 4 + 5))
        CS_sau((Thặng dư tiêu dùng sau: 1 + 2))
        PS_sau((Thặng dư sản xuất sau: 3))
        DWL_pc((Mất không ($DWL = 4 + 5$)))

        S --o E
        D --o E
        Pc --o Qd
        Pc --o Qs
        E --o P
        E --o Q
        Qd --o P
        Qs --o P
        ThieuHut --o Qd
        ThieuHut --o Qs

        style DWL_pc fill:#f9f,stroke:#333,stroke-width:2px
        style ThieuHut fill:#ccf,stroke:#333,stroke-width:2px
    end
