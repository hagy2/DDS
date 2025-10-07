---
title: Backups
parent: Technical Details
nav_order: 3
---

# Backups

This page documents backup experiments with YunoHost.

## Local backups
- Tested **YunoHost GUI → Backups**.
- Successfully created backups of apps.
- Verified that `.tar.gz` archives were stored locally.

## Remote backups (Borg)
- Attempted setup with **BorgBase** as remote backup target.

## Next steps
- Complete remote backup setup.
- Re-test Borg repo initialization.
- Explore alternative backup systems (e.g. rsync, Restic) in case Borg proves inaccessible.

---
📌 *Result:* Local backups work fine. Remote backups (with Borg) still need debugging.
