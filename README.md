# acc-releases

Internal release binaries for **ACC (Animatronics Control Center)**. This repository holds
signed installers and auto-update manifests only. It contains **no source code**.

- Published automatically by the release workflow in the (private) source repository.
- Each GitHub Release carries the Windows NSIS installer, its updater signature (`.sig`),
  `latest.json` and `latest.json.minisig`.
- All artifacts and manifests are verified by the app with minisign public keys compiled into it;
  files not signed by the ACC release key are rejected.
- Internal use only; not distributed in any store.
