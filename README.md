# System Design Handbook

A practical, open handbook for learning and revising **system design**: the core concepts, building blocks, trade-offs, and worked examples used to design scalable, reliable, and maintainable systems, and to prepare for system design interviews.

## Who is this for?

- Engineers preparing for system design interviews
- Developers moving from writing features to designing systems
- Anyone who wants a quick reference for distributed systems fundamentals

## Topics

Each topic lives in its own folder with a `README.md` and an `images/` folder for diagrams.

1. [Zero to Millions of Users](zero-to-millions-users/README.md)

### Planned topics

- Load balancers
- Caching
- Database replication and sharding
- Message queues
- Consistent hashing
- CAP theorem
- Rate limiter
- URL shortener
- News feed
- Chat application

## Repository layout

```
system-design-handbook/
├── README.md
└── zero-to-millions-users/
    ├── README.md
    └── images/
        ├── architecture.png
        └── scaling.png
```

## Adding a new topic

1. Create `topic-name/` with a `README.md` and an `images/` folder.
2. Explain the topic in `README.md` and keep all diagrams in `images/` with clear file names.
3. Add reference and source links at the end of the topic `README.md`.
4. Add the topic to the list above with a relative link.

## How to approach a design problem

1. **Clarify requirements**: functional and non-functional (scale, latency, availability).
2. **Estimate**: traffic, storage, and bandwidth.
3. **Define the API and data model.**
4. **Sketch the high-level design.**
5. **Deep dive** into the bottlenecks and critical components.
6. **Discuss trade-offs**, failure modes, and how the system evolves.

