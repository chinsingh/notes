# Transaction State

- **Active**: Transaction is going on
- **Partially committed**: After R/W operations
- **Failure**: Can go to this state from Active or from partially committed.
- **Aborted**: The step after failure
- **Committed**: The step after partially committed if storing permanently is successful - no rollback from here.
- **Terminated**: Transaction ended.
