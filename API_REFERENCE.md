# API reference

Mutexes and channels are opaque host handles. The portable wrappers enforce non-zero handles and a bounded channel capacity. Scheduling, blocking, fairness, and handle destruction remain host responsibilities and must be documented by each runtime adapter.

