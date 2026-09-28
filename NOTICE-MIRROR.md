# Notice — unmodified mirror

**This repository is not the MinIO project.** It is a fork of
[`minio/minio`](https://github.com/minio/minio), created on 2026-09-28 for a single purpose: to keep
the *corresponding source* of a container image mirror available.

## Why this fork exists

In September 2026 the official MinIO container images stopped resolving on both public registries
(Docker Hub returned 404 on the repository, quay.io returned `no such manifest` on the tag). A
private mirror of the already-pulled image was published to keep an existing deployment working.

MinIO Server is licensed under **AGPL-3.0-or-later**, and publishing that image is redistribution —
so the corresponding source has to remain reachable. It was pointed at `github.com/minio/minio`,
which is **archived**. A source pointer that depends on someone else's repository staying online is
not a pointer. This fork removes that dependency.

## What is mirrored

| | |
| --- | --- |
| Image | `ghcr.io/davidsondsf/minio` |
| Digest | `sha256:8631084d69dbc099ce362568ff3a24e1bd1ff1578bfb55d9dee2a2ef6bce1a7c` |
| Version | `RELEASE.2025-09-07T16-13-09Z` |
| Corresponding source | tag [`RELEASE.2025-09-07T16-13-09Z`](https://github.com/davidsondsf/minio/tree/RELEASE.2025-09-07T16-13-09Z), commit `01ce918d8279a20e4706b96a64396146894adee4` — identical to upstream |

The image is an **unmodified copy** of the official MinIO image, re-pushed to a reachable address.
No code was added, removed, or patched, and the original `LICENSE` is retained. The image keeps
MinIO's own OCI labels, including `org.opencontainers.image.licenses: AGPL-3.0-or-later` and
`vendor: MinIO Inc <dev@min.io>`.

## No affiliation

This mirror is **not affiliated with, endorsed by, or sponsored by MinIO, Inc.** "MinIO" is a
trademark of MinIO, Inc., used here only to identify the software being mirrored, as required to
state what the image contains.

If MinIO, Inc. would prefer this mirror renamed or taken down, please open an issue on this
repository — it will be honoured.
