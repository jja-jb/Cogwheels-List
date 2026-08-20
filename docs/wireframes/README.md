# Cogwheels List wireframes

These are control-plane wireframes for the surfaces described in
`10_specs/platform_support/013-ui-surfaces.txt`.

Cogwheel has no editing UI. Contacts.app is the human UI for contact, group,
membership, and photo data. None of these wireframes edits a contact or a
Sheet cell.

## Files

- [`01-first-launch.md`](01-first-launch.md) — first launch and setup states.
- [`02-authorization.md`](02-authorization.md) — Apple Contacts permission,
  Google account authorization, and Sheet picker states.
- [`03-main-status.md`](03-main-status.md) — idle, syncing, ok, blocked, and
  stopped status states.
- [`04-safety-states.md`](04-safety-states.md) — conflict freeze, size-bound
  fail-closed, second-instance fail-stop, and permission denial.
- [`05-reachability-diagnostics-recovery.md`](05-reachability-diagnostics-recovery.md)
  — Sheet unreachable, redacted diagnostics, and recovery.

## Shared frame

Every surface uses the same status frame:

```text
+--------------------------------------------------+
| Cogwheels List                         [status]  |
|--------------------------------------------------|
| Surface title                                    |
| State explanation                                |
|                                                  |
| [external/settings/retry route]    [Details]    |
|--------------------------------------------------|
| Contacts.app is the human editing surface.       |
+--------------------------------------------------+
```

`[Details]` exposes redacted diagnostics only. Labels such as “conflict field”
refer to a field name, never to the personal value stored in that field.
