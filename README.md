# saga-orchestration

Saga Orchestration is a pattern used in distributed transactions where multiple microservices must work together to complete a business process without using a traditional database transaction (no 2PC).

Instead of one big ACID transaction, the workflow is broken into local transactions, and if anything fails, the system performs compensating actions to undo the previous steps.
