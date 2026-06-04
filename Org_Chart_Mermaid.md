graph TD
    %% 스타일 설정
    classDef leader fill:#ff99ff,stroke:#9e9e9e,stroke-width:2px;
    classDef section fill:#c5c5fa,stroke:#9e9e9e,stroke-width:2px;
    classDef member fill:#f2e5bd,stroke:#9e9e9e,stroke-width:2px;

    %% 조직 구조 정의
    Leader[JV]:::leader

    %% 1. HW Maintenance Section
    HW[HW Maintenance Section]:::section
    B[Wella, the Boss Lady]:::member
    C[Anicko, the Hentai]:::member
    D[Edward, wala pang apelyido]:::member

    %% 2. SW Development Section
    SW[SW Development Section]:::section
    E[Jules...]:::member
    F[Sean the sheep]:::member

    %% Relationship
    Leader --> HW
    HW --> B
    HW --> C
    HW --> D

    Leader --> SW
    SW --> E
    SW --> F
