# Experiment Samples

## Turing Test Samples

Data for the Turing test. 

structure:
```
[
    {
        "nl": ... // natrual language utterance
        "is_people": ... // 1 or 0, 1 indicates human-generated
        "table": ... // table source. Sourced from nvBench if including `\\`, else from NLV Corpus. 
        "table_name": ... // table name. 
    }
]
```

## Comparative Study Samples


Data for comparative study. 

structure:
```
[
    {
        "table_name": "people", // table name, sourced from nvBench
        "database": "candidate_poll", //database, sourced from nvBench
        "rows_cnt": 9, // table rows count
        "cols_cnt": 6, // table cols count
        "data": [...], // table data
        "nl": "Compare males and females", // natrual language utterance
        "vis":{
            "1": { // vis id
                "vega": {...} , //Vega-lite spec
                "from": "chartgpt", // vis source, eg: chartgpt, nl4dv, ncNet
            },
        }
    },
    ...
]
```