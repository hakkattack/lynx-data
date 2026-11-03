# LYNX fantasy football report

`lynx_latest.json` contains the latest ESPN report for league **1818540**,
season **2026**, with **HakkAttack (team 8)** identified by `my_team_id`
and `my_team_name`. It uses the same report fields as WFFL.

On the configured Windows computer, run `C:\Users\Laptop\WFFL\run_lynx_daily.cmd`.
Each invocation retrieves ESPN data, writes the latest and dated snapshots
under `WFFL\snapshots`, updates `WFFL\lynx-data\lynx_latest.json`, commits
the report if changed, and pushes to GitHub. A failed export or push returns
a nonzero exit code. Logs are in `WFFL\logs\lynx_daily.log`.

The exporter shares the local `WFFL\espn_credentials.json` with WFFL.
Credentials must never be committed. Git must be authenticated for push.
WFFL's existing runner continues to operate separately.
