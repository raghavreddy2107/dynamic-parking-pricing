```mermaid
flowchart TD
    A[dataset.csv] --> B[Preprocessing]
    B --> C[Feature Engineering]
    C --> D[Pricing Models]
    D --> E[Competitor Adjustment]
    E --> F[Price Output]
    F --> G[Bokeh Plot]