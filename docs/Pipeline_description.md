# CircleCI Pipeline

[![CircleCI](https://dl.circleci.com/status-badge/img/circleci/Vjqo5kR5yPLNL7oBohMana/NZjzxdM483UB2TP9ceRydc/tree/master.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/circleci/Vjqo5kR5yPLNL7oBohMana/NZjzxdM483UB2TP9ceRydc/tree/master)

[![CircleCI](https://dl.circleci.com/insights-snapshot/circleci/Vjqo5kR5yPLNL7oBohMana/NZjzxdM483UB2TP9ceRydc/master/udagram/badge.svg?window=7d)](https://app.circleci.com/insights/circleci/Vjqo5kR5yPLNL7oBohMana/NZjzxdM483UB2TP9ceRydc/workflows/udagram/overview?branch=master&reporting-window=last-7-days&insights-snapshot=true)

## Configuration

Configuration file can be found at [config.yaml](../.circleci/config.yml)

Application Secrets are configured in Environment Variables section.
![](../screenshots/pipeline-env.png)

### Trigger

The CircleCi pipeline connected to github source
![](../screenshots/pipeline-source.png)

A push commit to `master` branch will trigger the pipeline.

## Workflow

The workflow has 3 jobs that run the scripts from [package.json](../package.json)

![](../screenshots/pipeline-workflow.png)

### 1. Build

install dependencies, lint, test and build
![](../screenshots/pipeline-build.png)

### 2. Hold

After build job, need manually approve to run deploy job.

### 3. Deploy

deploy web and api.
![](../screenshots/pipeline-deploy.png)
