# Failure Analysis Notes

## Task 001: Rolling Z-Score

This task evaluates whether an agent can implement a numerical rolling statistic robustly, not merely pass the obvious increasing-sequence case.

The public tests check basic behavior: simple rolling z-score computation and invalid window handling.

The hidden tests target common shallow-implementation failures:

- division by zero when the rolling standard deviation is zero
- incorrect handling of NaN values
- using the full history instead of the rolling window
- using sample standard deviation instead of population standard deviation
- failing when the window is larger than the input
- failing on negative values or degenerate inputs

This task is useful because many generated solutions can appear correct on simple examples while failing numerical edge cases.