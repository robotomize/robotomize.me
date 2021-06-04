+++
title = "Bloops"
+++

# Fliger.io


## What is fliger?
[Fliger.io](https://fliger.io) - 🐱‍🚀 An analytical web application for researching youtube comment reactions. 
The project uses neural networks to study emotional tone, entity extraction, and semantic analysis. 
This is a demo, it works with real data, but is limited to feature, code optimization, etc. 
Development is suspended

## Tech Stack
**Technology stack:** Go, Mongodb, ClickHouse, gRPC, Python, Flask, Vue.js, Bulma

## How it works?

Fliger works very simply. After a quick login, the user can search or analyze media by link. We use youtube api v3.
Data retrieval services download comments in the video that the user analyzes and store them in a clickhouse log for later processing.
The data services analyze the comments using flask+gRPC based machine learning and neural network models and store the enriched data.
Vue.js+bulma-based long polling clients query for data changes every n seconds.


##  Looks like
<img src="/img/fliger-2.gif" style="margin: 0;">
