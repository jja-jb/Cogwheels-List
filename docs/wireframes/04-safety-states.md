# Wireframe 04 — Safety and authorization states

## SF-01 — Conflict freeze

```text
+--------------------------------------------------+
| Cogwheels List                         FROZEN     |
|--------------------------------------------------|
| A field needs resolution                         |
| Field: <field name>                              |
| Cause: both sides changed from the ancestor      |
|                                                  |
| No automatic winner was selected.                 |
| Resolve the value in Contacts.app.               |
|                                                  |
| [Open Contacts.app] [Details]                    |
+--------------------------------------------------+
```

The wireframe names the field but does not display or edit either personal
value. There is no “choose left”, “choose right”, or in-app editor control.

## SF-02 — Size-bound fail-closed

```text
+--------------------------------------------------+
| Cogwheels List                         STOPPED    |
|--------------------------------------------------|
| Sync stopped before applying changes              |
| Reason: size bound exceeded                      |
| Result: fail-closed; no partial success          |
|                                                  |
| [Recovery] [Details]                              |
+--------------------------------------------------+
```

There is no override or partial-write action.

## SF-03 — Second-instance fail-stop

```text
+--------------------------------------------------+
| Cogwheels List                         STOPPED    |
|--------------------------------------------------|
| Another Cogwheel instance is active              |
| Reason: second-instance fingerprint              |
| Result: this instance will not sync              |
|                                                  |
| [Close this instance] [Details]                  |
+--------------------------------------------------+
```

The stopped instance exposes no control that resumes sync while the other
instance is present.

## SF-04 — Permission denied

```text
+--------------------------------------------------+
| Cogwheels List                         BLOCKED    |
|--------------------------------------------------|
| Authorization is required                         |
| Contacts: <Denied / Restricted>                   |
| Google:   <Denied / Unavailable>                  |
|                                                  |
| No data was synchronized.                         |
| [Open Settings] [Recovery] [Details]              |
+--------------------------------------------------+
```

Only the applicable denied source is named. The screen never substitutes a
missing source with stale or fabricated success.
