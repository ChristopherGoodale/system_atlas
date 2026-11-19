# System Atlas: live demo

**Open it:** https://christophergoodale.github.io/system_atlas/

System Atlas is an animated, explorable map of a home data and trading lab. It covers a financial data warehouse, a FIX trading simulator with its monitoring and alerting, and a small notification service. Data moves through it on a simulated clock. The screens:

- **Map:** every service, job, schema and link, with data moving along the links.
- **Tables:** the warehouse schemas, with table lineage and quality checks.
- **3D:** the major systems shown as floors of one building.
- **Tours:** five guided stories, such as the nightly load, a trading incident and an AI tool call.
- **Filters:** show one flow, one link type or a few systems at a time.

A generator reads the lab's own repositories (SQL migrations, transform SQL, Docker Compose, Prometheus config, schedulers) and writes the picture from them. It strips hostnames, private addresses and credentials before anything is published.

## Source code

This repository holds **only the built site**: minified JavaScript, CSS and a redacted `snapshot.json`. The generator, the app source and the tests are in a private repository. **They're available on request for review.**

Keys: `1`–`5` start a tour · `←`/`→` step · `Space` play/pause · `E` story/engineer · `M` map · `D` 3D · `T` tables · `F` full screen
