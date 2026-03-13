# PPC Monitor

This project monitors Google Ads campaign performance across accounts in an MCC.

The goal is to detect abnormal swings in campaign performance using trailing
7-day averages instead of fixed targets.

Metrics monitored:
- Spend
- Conversions
- CPA
- CTR
- CPC

Alerts will be delivered to Slack through an n8n workflow.
