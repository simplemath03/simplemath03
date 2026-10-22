# Jeffrey Campbell

Senior software engineer. Python, event-driven backends on Google Cloud, applied machine learning.
Rochester Hills, Michigan, working remotely.
[LinkedIn](https://www.linkedin.com/in/jeffrey-campbell-238955b6)

I build systems and then run them. At Ford I own an analytics platform end to end, from the
database and APIs to the roadmap, for about fifty engineers at sites around the world. On my own
time I build products that real people use every day, and I hold that work to the same bar:
automated tests, production telemetry, and a written record of every decision that mattered.

## Projects

**[NutriLog](https://github.com/simplemath03/nutrilog-architecture)**, an AI nutrition and
lifestyle coach, in production since June 2026. A React PWA talks to a FastAPI agent service,
which drives a Vertex AI model over about 35 tools exposed through a model-agnostic MCP server
backed by PostgreSQL. Cloud Run, Cloud SQL, Secret Manager, Cloud KMS, and Cloud Scheduler, all
in Terraform. Eight releases, 120+ automated tests, live LLM regression suites, and a 49-entry
decision log. The architecture repo has the full design and the decisions; source is available
on request.

**Zeus**, an event-driven algorithmic trading platform on GCP. Twelve Cloud Run services and
jobs communicate only through Pub/Sub with versioned JSON contracts: pre-market screeners,
a shared market-data ingestor, per-strategy engines, an execution manager, an IBKR bridge, a
portfolio monitor, and a BigQuery logger, with a fleet manager that wakes and sleeps the system
around market hours. The research side is a vectorized backtesting harness over 26M+ minute
bars and an event-study pipeline that evaluated 19 strategy families under pre-registered
rules; two survived. The repository is private. I am glad to walk through the architecture
and the research discipline in conversation.

**Test Data & Analytics Platform at Ford.** Database writes trigger Pub/Sub and Eventarc events,
Workflows route them to containerized Cloud Run services, results are written back and users
notified. It replaced a manual flash-drive-and-spreadsheet process and cut time to preliminary
results from over an hour to under ten minutes. Proprietary, so no code here.

## Publications and patent

Five peer-reviewed papers applying machine learning to EV battery systems:
[10.1109/ACCESS.2022.3208103](https://doi.org/10.1109/ACCESS.2022.3208103) ·
[10.4271/2022-01-0713](https://doi.org/10.4271/2022-01-0713) ·
[10.1109/EIT51626.2021.9491835](https://doi.org/10.1109/EIT51626.2021.9491835) ·
[10.4271/2021-01-1252](https://doi.org/10.4271/2021-01-1252) ·
[10.1109/ITEC51675.2021.9490081](https://doi.org/10.1109/ITEC51675.2021.9490081)

Patent [US11850968B2](https://patents.google.com/patent/US11850968B2): Compressing, Encrypting,
and Transmitting Battery Data in Vehicle.

## How I work

I use AI coding tools every day (Claude Code, Gemini CLI). They make me faster at the parts of
the job that were already mechanical. What they do not change is the standard: every change
ships with tests, production behavior is measured rather than assumed, and the reasoning behind
each decision is written down so the next person, including me in six months, can see why.

## Contact

j.campbell@utexas.edu
