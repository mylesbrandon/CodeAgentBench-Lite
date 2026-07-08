# Benchmark Task Guidelines

Each benchmark task should include:

1. A clear prompt/specification.
2. Starter code with the function signature.
3. A reference solution that passes all tests.
4. Public tests that check basic expected behavior.
5. Hidden tests that check edge cases and robustness.
6. Metadata describing the task category, difficulty, concepts, and targeted failure modes.

## Public vs Hidden Tests

Public tests should verify basic behavior and help clarify the task.

Hidden tests should check edge cases, boundary conditions, and failure modes that shallow implementations may miss.

Hidden tests should never check behavior that the prompt does not specify.

## Good Hidden Tests

A good hidden test is:
- fair
- tied to the written prompt
- narrow
- verifiable
- likely to catch a common incorrect implementation

## Bad Hidden Tests

A bad hidden test:
- checks an unstated requirement
- depends on subjective judgment
- has ambiguous expected behavior
- is too broad to diagnose