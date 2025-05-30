# Tutorial: allstars

AllStars helps you analyze data by providing a **Semantic Layer** that sits between your data and your queries. It defines *Metrics*, *Dimensions*, and *Relations* so you can ask questions in a simplified language. The system then *Transpiles* these requests into SQL that your *DatabaseInterface* can understand and execute.


**Source Repository:** [https://github.com/preset-io/allstars.git](https://github.com/preset-io/allstars.git)

```mermaid
flowchart TD
    A0["SemanticLayer
"]
    A1["Metric
"]
    A2["Dimension
"]
    A3["Relation
"]
    A4["Join
"]
    A5["Project
"]
    A6["Transpile
"]
    A7["DatabaseInterface
"]
    A5 -- "Manages" --> A0
    A0 -- "Contains" --> A3
    A0 -- "Contains" --> A4
    A0 -- "Contains" --> A1
    A0 -- "Contains" --> A2
    A5 -- "Uses" --> A7
    A7 -- "Provides metadata" --> A3
    A6 -- "Uses" --> A7
    A5 -- "Uses" --> A6
    A1 -- "Uses" --> A3
    A2 -- "Uses" --> A3
```

## Chapters

1. [Project
](01_project_.md)
2. [SemanticLayer
](02_semanticlayer_.md)
3. [Metric
](03_metric_.md)
4. [Dimension
](04_dimension_.md)
5. [Relation
](05_relation_.md)
6. [Join
](06_join_.md)
7. [Transpile
](07_transpile_.md)
8. [DatabaseInterface
](08_databaseinterface_.md)


---

Generated by [AI Codebase Knowledge Builder](https://github.com/The-Pocket/Tutorial-Codebase-Knowledge)