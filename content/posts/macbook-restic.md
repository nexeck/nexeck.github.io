---
draft: true
date: 2018-12-23T02:16:18+01:00
title: "MacBook Backup with Restic"
tags:
- MacBook
- macOS
- Mojave
categories:
- manual
---

```sh
$ export B2_ACCOUNT_ID=<MY_ACCOUNT_ID>
$ export B2_ACCOUNT_KEY=<MY_SECRET_ACCOUNT_KEY>
$ restic -r b2:beck-macos-backup init
```

```sh
$ restic -r b2:beck-macos-backup backup --tag initial --one-file-system --exclude-file=/Users/nexeck/.restic-exclude.list --exclude-caches /Users/nexeck
```


```sh
$ restic -r b2:beck-macos-backup
```


export B2_ACCOUNT_ID=0016d95e64f00310000000004
export B2_ACCOUNT_KEY=K001DLsKeBNC9CHHzs0V2qIUdDZvb6w

restic -r b2:beck-macos-backup backup --tag initial --one-file-system --exclude-file=/Users/nexeck/.restic-exclude.list --exclude-caches --force /Users/nexeck
