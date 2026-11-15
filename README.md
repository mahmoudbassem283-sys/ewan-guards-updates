# Ewan Guards signed updates

Current release: **4.9.2**, sequence **51**.

Owner update source:

```
https://raw.githubusercontent.com/mahmoudbassem283-sys/ewan-guards-updates/main/feed.json
```

Optional per-device Web Push notifications use the Ewan logo and program name. Each device requires an explicit enable action and browser permission. Alerts and the authenticated details page are filtered by current section permissions. Only encrypted count summaries are sent to the browser's push provider; names and national IDs are not included in Push payloads.

The host must remain online. Delivery after closing a page depends on browser/OS background support; force-stopping a browser can prevent delivery. iOS/iPadOS requires a supported Home Screen web app (16.4+). Provider acceptance of a test is not proof of device delivery; verify on the target device.

Validation: 180-test regression run, additional logout/lease/logo/native-click checks, 8 device-UI assertions, service-worker checks, cryptographic round-trip and VAPID verification, and actual supervised signed-upgrade/restart plus three start/stop cycles. Real Windows/mobile push receipt remains a device acceptance check.

The updater verifies the pinned signing key, package SHA-256, size and payload manifest. Packages are pinned to immutable commits. Installation remains an owner action inside the program.

This repository contains signed distribution packages only. No customer databases, account credentials, configuration, backups or private signing keys are published.
