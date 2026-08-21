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

## AU-04 — Create or join a shared Sheet

```text
+--------------------------------------------------+
| Sheet setup                                       |
|--------------------------------------------------|
| Target: <Create new Sheet / Choose existing>      |
|                                                  |
| First installation: create and manage the Sheet.  |
| Later installation: choose an existing shared    |
| Sheet using regular Google Sheet sharing.         |
|                                                  |
| [Create new Sheet] [Choose existing Sheet]        |
| [Details]                                         |
+--------------------------------------------------+
```

The create path uses the locked contacts, groups, membership, and photo
hash/presence schema. The join path selects an existing target and does not
create a new distributed lock or a spreadsheet editor. A second installation
has its own Apple and Google account; the same-fingerprint second-instance
fail-stop remains unchanged.

## AU-05 — Contacts container scope

```text
+--------------------------------------------------+
| Contacts source                                  |
|--------------------------------------------------|
| Read and write container: <iCloud / available>    |
|                                                  |
| Default: iCloud when available                    |
| Unified Contacts store: not selected              |
|                                                  |
| [Continue] [Details]                              |
+--------------------------------------------------+
```

Cogwheel uses one selected container as both the read set and write target. If
iCloud is absent, engineering selects among available containers with iCloud
preferred when available. The surface does not present the unified Contacts
store as a sync target.
