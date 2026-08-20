# Wireframe 02 — Authorization and Sheet selection

## AU-01 — Apple Contacts permission

```text
+--------------------------------------------------+
| Contacts permission                              |
|--------------------------------------------------|
| Cogwheel needs Contacts authorization to sync.    |
|                                                  |
| Permission: <Not determined / Requesting /        |
|              Authorized / Denied / Restricted>    |
|                                                  |
| [Request permission] [Open Settings] [Details]    |
+--------------------------------------------------+
```

`Authorized` proceeds to the next setup surface. `Denied` and `Restricted`
remain blocked; the screen does not display Contacts data.

## AU-02 — Google account authorization

```text
+--------------------------------------------------+
| Google account                                   |
|--------------------------------------------------|
| Connect the account used for the Sheet target.    |
|                                                  |
| Account: <Signed out / Authorizing / Authorized / |
|          Denied / Unavailable>                    |
|                                                  |
| [Connect Google] [Open Settings] [Details]        |
+--------------------------------------------------+
```

The account label is an authorization status, not a contact or Sheet editor.

## AU-03 — Sheet picker

```text
+--------------------------------------------------+
| Choose Sheet target                               |
|--------------------------------------------------|
| Google: Authorized                                |
|                                                  |
| Target: <None / Loading / Available / Selected>   |
|                                                  |
| [Choose Sheet] [Cancel] [Details]                 |
+--------------------------------------------------+
```

Picker states include `Unavailable` and `Cancelled`. A selected target is
shown as a redacted target identifier in diagnostics; this surface does not
show or edit cells.
