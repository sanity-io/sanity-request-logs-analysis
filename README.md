# Request log scripts

This repository contains a collection of scripts to help parse request logs. Reference: (https://www.sanity.io/docs/reference-request-log-data)[Request log scheme].

## Jupyter Notebook

Use ipython to interpret and visualize your data. See ./request-logs.ipynb

## JQ

Use the JQ command line tool to parse and filter log files

Example: `jq -c 'select(.attributes.sanity.endpoint == "query")' request-logs.ndjson > filtered_logs.ndjson`
