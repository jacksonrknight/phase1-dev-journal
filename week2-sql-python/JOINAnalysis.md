# Problem
Scenario: Your automation team needs to create a comprehensive server health report that correlates server performance, job failures, and alert generation patterns.

## Challenge
Write a query that shows:
- Server name
- Latest performance metrics (most recent CPU/memory readings)
- Number of failed automation jobs on that server
- Any alerts generated for that server
- Overall "health score" (custom calculation)

## Plan
- Need to filter by time
- all have server_name


### Tables I'm using
- performance_metrics (server performance over time)
- automation_jobs (job execution history)
- server_logs (server status and alerts)
#### table info 
performance_metrics:
- cpu & memory PERCENT
automation_jobs
- status
server logs
- cpu & mem USAGE
alert_level
status

### SQL

