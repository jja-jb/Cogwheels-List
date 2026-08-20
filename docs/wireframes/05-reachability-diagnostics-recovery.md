# Wireframe 05 — Reachability, diagnostics, and recovery

## RC-01 — Sheet unreachable

```text
+--------------------------------------------------+
| Cogwheels List                         BLOCKED    |
|--------------------------------------------------|
| Sheet cannot be reached                           |
| Last known outcome: <redacted status>             |
| Current run: not successful                       |
|                                                  |
| [Retry] [Recovery] [Diagnostics]                  |
+--------------------------------------------------+
```

Retry is a reachability route, not a Sheet editor. The screen does not claim
success while the Sheet is unreachable.

## RC-02 — Diagnostics

```text
+--------------------------------------------------+
| Diagnostics                                       |
|--------------------------------------------------|
| Run state:       <redacted state>                 |
| Reason code:     <redacted code>                  |
| Last run:        <timestamp>                     |
| Contacts:        <available / blocked>            |
| Sheet:           <available / unreachable>         |
| Instance safety: <clear / stopped>                |
| Size bound:      <clear / exceeded>               |
| Conflict fields: <field names only>               |
|                                                  |
| Personal data: redacted                           |
| [Back] [Recovery]                                 |
+--------------------------------------------------+
```

Diagnostics may show state, reason codes, timestamps, source availability,
instance safety, size-bound state, and conflict field names. They omit or
redact personal names, emails, phone numbers, addresses, raw contact payloads,
Sheet cell values, access tokens, and photo bytes.

## RC-03 — Recovery

```text
+--------------------------------------------------+
| Recovery                                         |
|--------------------------------------------------|
| Blocked condition: <authorization / reachability |
|                    / conflict / size / instance> |
|                                                  |
| Next external action: <settings / Contacts.app / |
|                       retry / close instance>     |
|                                                  |
| This surface cannot edit data or bypass safety.   |
| [Take external action] [Back] [Diagnostics]       |
+--------------------------------------------------+
```

Recovery is reason-specific. Conflict recovery points to Contacts.app; it does
not resolve a named field inside Cogwheel. Size-bound and second-instance
states remain fail-closed/fail-stop until their condition is cleared.
