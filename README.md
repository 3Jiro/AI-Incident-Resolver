# 🛡️ AI Incident Resolver & Self-Healing Audit System

# 🌟 Overview
A "DevOps-in-a-Box" solution designed to automate Tier-1 incident response. This workflow monitors service webhooks, diagnoses the root cause using an LLM-powered "Rule Book" lookup, and executes corrective actions (Restarts/Scaling) autonomously.

# 🛠️ Technical Architecture
- Anomaly Verification: Cross-references incoming incident data against a Google Sheets "Historical Log" to identify recurring patterns.

- Audit-Trail Logging: Every autonomous action is logged with a dual-entry system (Slack for immediate visibility and Google Sheets for long-term reporting).

- Gemini Logic Engine: Uses a dedicated "Workflow Auditor" node to analyze post-incident logs for operational anomalies.

# 🚀 Key Challenges Overcome
- False Positive Filtering: Implemented a multi-stage "Logic Filter" that prevents the AI from triggering service restarts for non-critical warnings.

- Regulatory Compliance: Designed the system to provide a full "Explanation of Action" in Slack, ensuring human oversight of every automated fix.
