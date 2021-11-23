+++ title = "Bloops"
+++

# Fliger

Fliger is a project I came up with by accident and developed a prototype in 3 days. In 2019 we developed a demo version
during a month-long vacation with [Polina Galanina](https://www.behance.net/polberry), which we showed to friends in the
blogging community. The project was frozen due to lack of ideas for monetization and further development.

## What is fliger.io?

[Fliger.io](https://fliger.io) - 🐱‍🚀 An analytical web application for researching youtube comment reactions. The
project uses neural networks to study emotional tone, entity extraction, and semantic analysis. This is a demo, it works
with real data, but is limited to feature, code optimization, etc.

## Tech Stack

**Technology stack:** Go, Mongodb, ClickHouse, gRPC, Python, Flask, Vue.js, Bulma

## How it works?

Fliger works very simply. After a quick login, the user can search or analyze media by link. We use youtube api v3. Data
retrieval services download comments in the video that the user analyzes and store them in a clickhouse log for later
processing. The data services analyze the comments using flask+gRPC based machine learning and neural network models and
store the enriched data. Vue.js+bulma-based long polling clients query for data changes every n seconds.

## Looks like

<img src="/img/fliger-2.gif" style="margin: 0;">
