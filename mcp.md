# mcp.md
## Connecting the dayNumber_ MCP

The dayNumber_ MCP server gives this coach direct access to your logs. Without it the coach is reading what you paste. With it the coach is reading your actual journey.

---

## Setup

In your Claude project settings, under Connections or MCP Servers, add:

- Name: dayNumber_
- URL: https://mcp.daynumber.io/mcp

Save and start a new conversation. The coach will automatically have access to your logs.

---

## What the coach can see with MCP connected

- Your day # — calculated from your actual startup start date
- Your last 30 logs — full text, dates, day numbers
- Your consistency signal — green, amber, or red based on your last 7 days
- Your morning brief — day #, streak, what happened recently
- The network — other founders building publicly on dayNumber_, their patterns and themes

---

## What the coach cannot see

- Your email or payment information
- Any private fields on your profile
- Logs from founders who have not made their profile public

---

## Tools available to the coach

- `read_logs` — reads your own logs (authenticated)
- `read_founder_logs` — reads any public founder's logs by username
- `get_morning_brief` — your current day #, streak, and recent summary
- `get_network_signal` — query the entire founder network
- `get_community` — community stats if you are in one
- `post_log` — log today's entry directly from Claude
- `query_journey` — AI-powered query across your full log history

---

## Troubleshooting

If the coach says it cannot access your logs, disconnect and reconnect the MCP server in your Claude project settings. The connection occasionally needs a refresh after inactivity.
