        +--------+
        | Source |
        +--------+
            |
            v
        +--------+
        |  Task  |
        | Queue  |
        +--------+
            |
            v
+-----------+  +-----------+  +-----------+
|  Worker   |  |  Worker   |  |  Worker   |
| Goroutine |  | Goroutine |  | Goroutine |
+-----------+  +-----------+  +-----------+
            |       |         |
            |       |         |
            v       |         |
        +--------+  |         |
        |  Task  |  |         |
        |  Queue |  |         |
        +--------+  |         |
            |       |         |
            v       v         v
        +--------+  +-----------+
        | Result |  |  Result   |
        | Queue  |  |  Queue    |
        +--------+  +-----------+
