sequenceDiagram
    Channel App->>Search src: Search
    Search src->>product index: Lookup
    product index->>Search src: 
    Search src->>inventory src: availability check
    inventory src->>Search src: 
    Search src->>Search src: Product list process
    Search src->>Channel App: Searches
    Note left of Channel App: render