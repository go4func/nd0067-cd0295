# CircleCI Pipeline

[![CircleCI](https://dl.circleci.com/status-badge/img/circleci/Vjqo5kR5yPLNL7oBohMana/NZjzxdM483UB2TP9ceRydc/tree/master.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/circleci/Vjqo5kR5yPLNL7oBohMana/NZjzxdM483UB2TP9ceRydc/tree/master)

[![CircleCI](https://dl.circleci.com/insights-snapshot/circleci/Vjqo5kR5yPLNL7oBohMana/NZjzxdM483UB2TP9ceRydc/master/udagram/badge.svg?window=7d)](https://app.circleci.com/insights/circleci/Vjqo5kR5yPLNL7oBohMana/NZjzxdM483UB2TP9ceRydc/workflows/udagram/overview?branch=master&reporting-window=last-7-days&insights-snapshot=true)

## Configuration

Configuration file can be found at [config.yaml](../.circleci/config.yml)

## Workflow

The workflow has 3 jobs that run the scripts from [package.json](../package.json)

- build: install dependencies, lint, test and build
- hold: manually approve to proceed to build jobs.
- deploy: deploy web and api.

After build job, need manually approve to run deploy job.

### Trigger

A push commit to `master` branch will trigger the pipeline.

## Screenshot

![](../screenshots/pipeline-1.png)
![](../screenshots/pipeline-2.png)
![](../screenshots/pipeline-3.png)
![](../screenshots/pipeline-4.png)
