<div align="center">
  </a>
</div>

# Decentralized Longevity Research A.I. Agent

Can an Optimized Reasoning Engine
every single research paper published

**This project is not affiliated with any platform.**

## Setup

Run the following command:

```sh
run 1
```

## What's inside?

This repo is a monorepo managed by L.O.R.E


### Build

To build the web app, run the following command:

```
turbo build
```

### Develop

To develop the web app, run the following command:

```
turbo dev
```

## The Pipeline
The pipeline is current running on a cron job.
1. The agent is running every 24 hours.
2. Then with the Batch API from OpenAI, we analyze if the paper is relevant to our L.O.R.E protocol.
3. Store the results in the Postgres database.
4. Finally, we only process the relevant papers to the final pipeline to get the results.
5. The results are then displayed on the web app.

## The Agent
The agent has two functions

### 1. Chat
The agent will answer all your question.

### 2. Twitter Automation
Whenever someone tweets at the agent about L.O.R.E, the agent will respond with a response.
In the future, I will add LORE functionality to the agent so that it can generate responses based on the research papers.

## Roadmap
1. Automate the tweet selection process
2. Add LORE functionality to the agent
3. Add more data sources to the pipeline (PubMed, etc...)
4. Add more functionality to the web app (search, filter, etc...)

