## My internship work (Fall 2026)

Completed all four maintenance tickets on Sweet Home 3D 5.4, a ~94k-line legacy Java Swing
codebase, using a branch-per-task workflow with GitHub Issues.

| Task | Change | Key files |
| --- | --- | --- |
| 1 | Built and ran the legacy app with Maven on JDK 8 | `pom.xml` |
| 2 | Made furniture descriptions editable by changing the controller's editability rule | `HomeFurnitureController` |
| 3 | Added a sortable, toggleable **Volume** column (width × depth × height) across model, controller, view and i18n resources | `HomePieceOfFurniture`, `HomePane`, `FurnitureTable`, `package.properties` |
| 4 | Printing now outputs every viewable level: an all-level furniture table with a Level column, then one plan page per level, restoring the user's selected level via `try/finally` | `PlanComponent`, `HomePrintableComponent`, `FurnitureTable` |

**What I practised:** tracing an existing feature through MVC layers, extending enum-driven
designs (Strategy-style comparator map), handling temporary state safely, and keeping UI
strings in resource bundles.

Acceptance evidence is in [`submissions/`](submissions/). All provided tests pass (`mvn test`).

---
