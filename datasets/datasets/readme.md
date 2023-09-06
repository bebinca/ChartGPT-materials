# Datasets

The table data files are provided by nvBench. 

We only include the utterance, chart template answers, and its related database / table names here. 

## Data Configuration

`train_set.csv` and `test_set.csv` follow the same configuration: 

| Attribute | Description |
|-----------|-------------|
| nl | The natrual language utterance.  |
| nl type | `abstract` (generated) or `original` (sourced from nvBench). |
| chart | Chart type. |
|hardness| Hardness level of generating the chart. Sourced from nvBench. |
|table name| Table name. Sourced from nvBench. |
|database| Database name. Sourced from nvBench. |
|label| Chart specification in Vega-Zero. Sourced from nvBench. |
|column| Step 1. Select columns.  |
|filter| Step 2. Add filter. |
|aggregate| Step 3. Add aggregations. |
|mark| Step 4. Select chart type. |
|encoding| Step 5. Choose encoding. |
|sort| Step 6. Add sort. |