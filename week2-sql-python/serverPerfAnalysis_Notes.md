# Problem
Scenario: Your automation team needs to identify performance patterns. Management wants to know which servers have the highest average resource usage and during which time periods they peak.

## Challenge
Write a Query that shows:
- Server name
- Average CPU and memory usage
- Peak CPU time (when CPU was highest)
- Total number of monitoring records per server

## Plan

- server name will be main select
- avg(cpu_percent), avg(memory_percent)
    - group it all by server_name
- will have to select timestamp for max(cpu_percent)
- count of records per server

### SQL
SELECT p.server_name, p.cpu_avg, p.mem_avg,
	(SELECT p2.timestamp
	 FROM performance_metrics p2
	 WHERE p2.server_name = p.server_name
	 ORDER BY p2.server_name DESC
	 LIMIT 1
	) peak_cpu_time
-- Now need to pull for the averages, make another query that averages each and sends it back. Will run for each group by 
FROM (
	SELECT server_name, AVG(cpu_percent) AS cpu_avg, AVG(memory_percent) AS mem_avg
	FROM performance_metrics
	GROUP BY server_name
	) p
;
	