```mermaid
flowchart TD
    %% --- [1. 조직도 구조 정의] ---
    A["Team lead<br/><b>A</b>"]:::lead
    
    HW["1. HW Maintenance<br/><b>Section</b>"]:::hw
    SW["2. SW Development<br/><b>Section</b>"]:::sw
    
    B["<b>B</b>"]:::hw
    C["<b>C</b>"]:::hw
    D["<b>D</b>"]:::hw
    
    E["<b>E</b>"]:::sw
    F["<b>F</b>"]:::sw

    %% --- [2. 조직도 연결 관계] ---
    A --- HW
    A --- SW
    HW --- B
    HW --- C
    HW --- D
    SW --- E
    SW --- F

    %% --- [3. 하단 범례] ---
    subgraph 범례 [" "]
        direction LR
        L1["　"]:::lead ~~~ T1["Team lead"]:::txt
        L2["　"]:::hw  ~~~ T2["HW Maintenance"]:::txt
        L3["　"]:::sw  ~~~ T3["SW Development"]:::txt
    end

    %% --- [4. 스타일 및 색상 정의] ---
    classDef lead fill:#3B3688,stroke:none,color:#FFFFFF,border-radius:10px;
    classDef hw fill:#034A3E,stroke:none,color:#FFFFFF,border-radius:10px;
    classDef sw fill:#6A2C11,stroke:none,color:#FFFFFF,border-radius:10px;
    classDef txt fill:none,stroke:none,color:#555555,font-weight:bold;

    linkStyle 0,1,2,3,4,5,6 stroke:#E0E0E0,stroke-width:2px;
    style 범례 fill:none,stroke:none;
