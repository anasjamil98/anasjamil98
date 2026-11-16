# Anas Jamil

Data Analytics Manager in fintech. Central-bank regulatory reporting, payments and transaction data, BI and ETL. I own the context engineering behind an approved AI query assistant in production.

SQL · Python · Power BI

Most of the job isn't the query. It's finding the question underneath the request, because two teams can ask for "active users" and mean two different things, and whichever one you answer first becomes the number everybody quotes for the next year.

## Projects

Each of these takes a problem I work on and rebuilds the approach from scratch, on synthetic data for a fictional digital wallet. None of it is my employer's code or data.

| Project | The problem | What to look at |
|---|---|---|
| [regulatory-return-automation](https://github.com/anasjamil98/regulatory-return-automation) | A regulatory return assembled by hand fails on the month you can't afford it to | Ten blocking controls, a control total computed by a second route, and an audit record for every run, including the blocked ones |
| [aliased-sql-assistant](https://github.com/anasjamil98/aliased-sql-assistant) | Getting AI into a regulated environment is an architecture problem, not a prompting one | A model that never sees a real table name or a row of data, a context file tested like code, and an eval showing what guardrails can't catch |
| [metrics-source-of-truth](https://github.com/anasjamil98/metrics-source-of-truth) | Two teams ask for "active users" and mean two different things | One question with six defensible answers, metric contracts that can't drift from the tables, and an alert that was wrong twice before it was right |
| [year-in-review-etl](https://github.com/anasjamil98/year-in-review-etl) | A personalised summary goes to every customer at once, and each of them knows their own numbers | Four card variants for the customers a standard card doesn't fit, and every metric computed twice by code that shares nothing |
| [single-file-exec-dashboard](https://github.com/anasjamil98/single-file-exec-dashboard) | Leadership wants to explore the numbers without a licence, a login or a VPN | An interactive dashboard in one 88 KB HTML file, with small cells folded before the data is written |

They share one dataset: about 195,000 transactions for 4,000 invented customers, generated from a fixed seed. It's built to be awkward in the ways payments data is. Timestamps are in UTC while the business reports in local time, amounts are in minor units, test accounts transact like real ones, and one day has an outage.

All five run on Python 3.9 with SQLite, so there's nothing to provision. Every repo has tests, and every README has a section on what went wrong or what I'd change.

The portfolio site, with the dashboard running live, is at [anasjamil98.github.io](https://anasjamil98.github.io).

## Day to day

Three things take up most of my week at NayaPay.

**Regulatory reporting.** I build and automate the data behind our central-bank submissions. Compliance files them, I make sure what they're filing is right.

**AI tooling.** I own the AI query assistant our data team runs on, approved by our Head of Data. It sits on an aliased warehouse layer so the model never sees real table names or customer data, an approach I took to our security team before we built anything.

**Definitions.** MAU, DAU, TPV, wallet states. I built the source-of-truth tables and the documentation behind them, because that knowledge was living in two people's heads.

Before this, two years at eZhire building BI for the GCC market, and before that a technical business analyst at Wavetec, deploying for banks including HSBC, Banorte and BBVA. Databases first, dashboards later.

## Tools

SQL and Trino, Python, Jupyter and pandas, Power BI, Looker Studio, Excel.

## Contact

[LinkedIn](https://www.linkedin.com/in/anasjamilaj) · anas_jamil@live.com

Views here are my own and not my employer's.
