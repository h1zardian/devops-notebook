---
id: gm4dqh9xz4q63l8xuupnbgm
title: Azure File Storage
desc: ''
updated: 1655019371070
created: 1653661331066
---

* File Storage is semantically identical to [[Blob Storage|cloud-concepts.azure.services.storage.azure-blob-storage]], with notable differences.

  * Instead of BLOBS you store files
  * Instead fo containers, files are stored in `shares`
  * The file storage is accessed via `SMB` protocol,  
    (Server Message Block) is a shared drive protocol.


* Great implementation for lift-and-shift scenarios.
