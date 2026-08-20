# Wireframe 03 — Main status

## ST-01 — Idle / not configured

```text
+--------------------------------------------------+
| Cogwheels List                         IDLE       |
|--------------------------------------------------|
| Sync is not running                              |
| Setup is incomplete: <reason>                    |
|                                                  |
| Contacts       <authorized / blocked>            |
| Google         <authorized / blocked>            |
| Sheet          <selected / not selected>         |
|                                                  |
| [Setup] [Diagnostics]                             |
+--------------------------------------------------+
```

## ST-02 — Syncing

```text
+--------------------------------------------------+
| Cogwheels List                         SYNCING    |
|--------------------------------------------------|
| Sync in progress                                 |
| Stage: <reading / comparing / applying /         |
|         verifying>                               |
|                                                  |
| Safety: <clear / blocked>                         |
|                                                  |
| [Diagnostics]                                    |
+--------------------------------------------------+
```

## ST-03 — Ok

```text
+--------------------------------------------------+
| Cogwheels List                         OK         |
|--------------------------------------------------|
| Latest run completed successfully                 |
| Last result: OK                                  |
|                                                  |
| Contacts       Available                         |
| Google         Available                         |
| Sheet          Selected                          |
|                                                  |
| [Diagnostics]                                    |
+--------------------------------------------------+
```

## ST-04 — Blocked or stopped

```text
+--------------------------------------------------+
| Cogwheels List                  <BLOCKED/STOPPED> |
|--------------------------------------------------|
| Sync did not proceed                             |
| Reason: <named state>                            |
| No successful result was recorded for this run.   |
|                                                  |
| [Recovery] [Diagnostics]                          |
+--------------------------------------------------+
```

The state name is one of the defined authorization, reachability, conflict,
size-bound, or instance-safety conditions. No contact or Sheet editing control
appears in any state.
