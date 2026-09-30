# Validation roadmap

The tasks below are planned work, **not completed controls**.

1. Recheck current service state and agent connectivity after the September baseline.
2. Produce a harmless endpoint action and trace its event with timestamps at source and in Wazuh. Record whether a rule fires or only the source event is visible.
3. Identify intended administrator and agent access paths; test both an approved path and a denied path before claiming restricted access.
4. Record service and disk health over multiple days and choose a retention goal based on measured growth.
5. Create a protected off-host backup and verify a limited restore into a disposable location.
6. Stop and restart the agent in a controlled exercise, record the alerting gap and confirm recovery.

For each test, capture the date, command or action, expected result, actual result, a redacted evidence reference and the limitation. Avoid publishing live credentials or raw authentication logs.
