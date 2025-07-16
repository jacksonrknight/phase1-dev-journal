# Problem
Scenario: Your automation system needs to identify "problem hours" - time periods when multiple servers are under stress simultaneously.

## Challenge
Write a Query that shows:
- Each hour of the day
- How many servers had CPU > 80% during that hour
- Average memory usage across all servers for that hour
- List the server names that were stressed (CPU > 80%) during each hour

## Plan
- will be GROUP BY hour


### SQL
 SELECT 
	strftime('%H', timestamp) AS hour,
	COUNT(CASE WHEN cpu_percent > 80 THEN 1 ELSE NULL END) AS server_count,
	AVG(memory_percent) AS avg_mem,
	GROUP_CONCAT(CASE WHEN cpu_percent > 80 THEN server_name ELSE NULL END, ', ') AS stressed_servers
FROM performance_metrics
GROUP BY strftime('%H', timestamp)
;
