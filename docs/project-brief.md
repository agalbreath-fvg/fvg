# Project Brief

Build a PPC monitoring system for Google Ads using an MCC.

## Objective
Detect abnormal swings in campaign performance using trailing 7-day averages instead of fixed targets.

## Accounts
The system should only monitor a predefined list of Google Ads accounts under the MCC.
Not all linked accounts should be included.

The monitored accounts will be defined in a configuration list.

## Scope
The system should:
- check only the configured accounts
- analyze campaign-level metrics
- compare yesterday vs trailing 7-day average
- flag abnormal swings
- send a daily Slack update via n8n

## Metrics
- Spend
- Conversions
- CPA
- CTR
- CPC

## Output
The system should send a daily Slack summary even if no major issues are found.

The summary should:
- highlight abnormal swings or possible issues
- note campaigns or accounts that appear stable
- confirm when everything looks normal

The goal is to provide visibility every day, not only when something is wrong.
