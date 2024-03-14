# Request log scripts

This repository is intended to contain a collection of scripts to help parse request logs. Reference: [Request log schema](https://www.sanity.io/docs/reference-request-log-data).
More scripts will be added over time. 

PR's welcome!

## Jupyter Notebook

Use ipython to interpret and visualize your data. See ./request-logs.ipynb

## JQ

Use the JQ command line tool to parse and filter log files

Example: `jq -c 'select(.attributes.sanity.endpoint == "query")' request-logs.ndjson > filtered_logs.ndjson`
