# Architecture

Cogwheel's List is a macOS relay with three bounded responsibilities:

1. Read the configured Apple Contacts source.
2. Read and write the specified Google Sheet through the user's authorized account.
3. Reconcile changes and report sync state without becoming a second editing surface.

The Contacts and Google Sheet sources remain the homes of user data. Authentication, field mapping, conflict policy, durable sync checkpoints, and error recovery are specified in numbered documents under `10_specs/platform_support/`.
