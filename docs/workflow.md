# Workflow

This project is a Google Ads PPC monitor for selected accounts under an MCC.

## Daily Process
1. Read the list of monitored accounts from the config file.
2. Pull campaign-level Google Ads metrics for each selected account.
3. Pull yesterday's metrics for:
   - Spend
   - Conversions
   - CPA
   - CTR
   - CPC
4. Pull the trailing 7-day average for the same metrics.
5. Compare yesterday against the trailing 7-day average.
6. Apply the alert rules.
7. Build a daily summary.
8. Send the summary to Slack through n8n.

## Output Expectations
The system should send a daily Slack update even if no major issues are found.

If metrics look stable, say so.
If metrics show abnormal swings, flag them clearly.
