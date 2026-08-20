# Wireframe 01 — First launch and setup

## FL-01 — Not started

```text
+--------------------------------------------------+
| Cogwheels List                         NOT SET UP |
|--------------------------------------------------|
| Set up sync                                      |
| Cogwheel uses Contacts.app for editing.          |
| Choose authorization sources to continue.        |
|                                                  |
| Contacts permission       Not requested          |
| Google account            Not connected          |
| Sheet                      Not selected          |
|                                                  |
|                         [Begin setup]             |
+--------------------------------------------------+
```

The screen introduces the product boundary and does not show contact or Sheet
rows.

## FL-02 — Setup in progress

```text
+--------------------------------------------------+
| Cogwheels List                         SETTING UP |
|--------------------------------------------------|
| Preparing authorization                           |
|                                                  |
| Contacts permission       In progress             |
| Google account            Not started             |
| Sheet                      Not started             |
|                                                  |
|                         [Cancel setup]            |
+--------------------------------------------------+
```

## FL-03 — Ready for authorization

```text
+--------------------------------------------------+
| Cogwheels List                         READY      |
|--------------------------------------------------|
| Finish setup to enable sync                       |
|                                                  |
| Contacts permission       Needs authorization     |
| Google account            Needs authorization     |
| Sheet                      Needs selection        |
|                                                  |
| [Authorize Contacts]  [Connect Google]            |
+--------------------------------------------------+
```

## FL-04 — Setup blocked

```text
+--------------------------------------------------+
| Cogwheels List                         BLOCKED    |
|--------------------------------------------------|
| Setup cannot continue                             |
| Reason: <authorization or safety reason>         |
| No data was synchronized.                         |
|                                                  |
| [Open external recovery route]       [Details]    |
+--------------------------------------------------+
```

The reason is supplied by the applicable authorization or safety state. The
screen never offers an override or a data-editing action.
