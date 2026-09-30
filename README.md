# System Design Handbook

A practical, open handbook for learning and revising **system design**: the core concepts, building blocks, trade-offs, and worked examples used to design scalable, reliable, and maintainable systems, and to prepare for system design interviews.

## Who is this for?

- Engineers preparing for system design interviews
- Developers moving from writing features to designing systems
- Anyone who wants a quick reference for distributed systems fundamentals

## Contents

### 1. Fundamentals
- Scalability (vertical vs. horizontal)
- Latency, throughput, and availability
- Reliability, fault tolerance, and redundancy
- CAP theorem and PACELC
- Consistency models (strong, eventual, causal)

### 2. Building Blocks
- Load balancers
- Reverse proxies and API gateways
- Caching (CDN, in-memory, write-through, write-back, eviction policies)
- Databases (SQL vs. NoSQL, indexing, replication, sharding, partitioning)
- Message queues and event streaming
- Object and blob storage
- Search systems

### 3. Communication and APIs
- REST, gRPC, GraphQL
- WebSockets, long polling, server-sent events
- Rate limiting and throttling
- Idempotency and API versioning

### 4. Distributed Systems Concepts
- Consensus (Paxos, Raft)
- Leader election
- Consistent hashing
- Distributed transactions (2PC, saga)
- Clocks and ordering
- Service discovery

### 5. Architecture Patterns
- Monolith vs. microservices
- Event-driven architecture
- CQRS and event sourcing
- Pub/sub
- Back pressure and circuit breakers

### 6. Observability and Operations
- Logging, metrics, tracing
- Monitoring and alerting
- Deployment strategies (blue/green, canary)
- Disaster recovery

### 7. Security
- Authentication and authorization
- Encryption in transit and at rest
- Common attack mitigations

### 8. Case Studies
Worked designs, each with requirements, estimation, high-level design, deep dives, and trade-offs:
- URL shortener
- Rate limiter
- News feed
- Chat application
- Video streaming platform
- Ride-hailing service
- Distributed cache
- Notification system

## Repository layout

Each topic lives in its own folder with a `README.md` and an `images/` folder for diagrams:

```
system-design-handbook/
├── README.md
├── zero-to-million-users/
│   ├── README.md
│   └── images/
├── consistent-hashing/
│   ├── README.md
│   └── images/
└── ...
```

## How to approach a design problem

1. **Clarify requirements**: functional and non-functional (scale, latency, availability).
2. **Estimate**: traffic, storage, and bandwidth.
3. **Define the API and data model.**
4. **Sketch the high-level design.**
5. **Deep dive** into the bottlenecks and critical components.
6. **Discuss trade-offs**, failure modes, and how the system evolves.

## Contributing

Contributions are welcome: fixes, new topics, diagrams, and case studies.

1. Fork the repository
2. Create a branch (`git checkout -b topic/my-change`)
3. Commit your changes and open a pull request

## License

To be decided. Add a `LICENSE` file to specify how this content may be used.
