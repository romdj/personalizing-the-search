graph TD
    A1{Website} --- B(Search API)
    A2{Application} --- B(Search API)
    B --> C(Search Capability)
    C --> E(Product Data System)
    C --> B
    E --> C
    E --> F1[(product data)]
    E --> F2[(product tagging)]
    E --> F3[(inventory)]
    F1 --> E
    F2 --> E
    F3 --> E