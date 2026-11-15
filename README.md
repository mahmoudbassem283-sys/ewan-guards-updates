# Ewan Guards signed updates

Public distribution of signed EwanGuardsSystem update packages only.

Current release: **4.9.1**, sequence **50**.

Update source:

```
https://raw.githubusercontent.com/mahmoudbassem283-sys/ewan-guards-updates/main/feed.json
```

The installed updater verifies the release signature against its pinned public key, package size and SHA-256, and every payload file before installation. The package URL is pinned to an immutable commit. Installation remains an owner action inside the program.

No customer database, account credentials, runtime configuration, backups, or private signing key belongs in this repository.
