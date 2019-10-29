# Crunchbase DB (2013)

Includes data dump (in `./data`) from historical Crunchbase DB.

See https://data.crunchbase.com/docs/2013-snapshot for more info. 

## Database Schema

![Crunchbase DB Schema](data/schema.png?raw=true "Crunchbase DB Schema")

## Getting started

Ingest the data files into your own MySQL database (e.g. `crunchbase`) using the following command – _order matters!_:

```bash
% mysql crunchbase < ./data/cb_objects.sql
% mysql crunchbase < ./data/cb_acquisitions.sql
% mysql crunchbase < ./data/cb_degrees.sql
% mysql crunchbase < ./data/cb_funding_rounds.sql
% mysql crunchbase < ./data/cb_funds.sql
% mysql crunchbase < ./data/cb_ipos.sql
% mysql crunchbase < ./data/cb_milestones.sql
% mysql crunchbase < ./data/cb_offices.sql
% mysql crunchbase < ./data/cb_people.sql
% mysql crunchbase < ./data/cb_investments.sql
```
