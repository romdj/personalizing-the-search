sequenceDiagram
    Channel App->>Search src: Search
    Search src->>product family index (Graph DB): Lookup
    product family index (Graph DB)->>Search src: 
    Search src->>inventory src: availability check
    inventory src->>Search src: 
    Search src->>Search src: Product list process
    Search src->>Search src: Reinforcement Learning Algorithm
    Search src->>Channel App: Searches
    Note left of Channel App: render