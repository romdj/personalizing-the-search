graph TD
    A1{Website} --- B(Search API)
    A2{Application} --- B(Search API)
    B --> RL(Reinforcement Learning algorithm)
    RL --> B
    DL(Data Lake) --> AL(Analytics Feedback)
    AL(Analytics Feedback) --> RL
    B --> C(Search Capability)
    C --> GPPR(Search Product matching DB)
    C --> GPPE(Search Persona matching DB)
    GPPR --> C
    GPPE --> C
    C --> E(Product Data System)
    C --> B
    E --> C
    M1 --> F1[(product data)]
    E --> M1(Marketing Campaign management system)
    M1 --> E
    M1 --> F2[(product tagging)]
    E --> F3[(inventory)]
    F1 --> M1
    F2 --> E
    F2 --> GPPR
    F3 --> E