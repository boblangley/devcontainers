# Dev containers

Dev Container images, Templates, and Features published by Bob Langley to GitHub Container Registry.

## Ubuntu image

`ghcr.io/boblangley/devcontainers/base` derives from Microsoft's Ubuntu Dev Container base and adds s6-overlay as PID 1.

Supported rolling tags:

- `noble` and `ubuntu24.04`
- `resolute` and `ubuntu26.04`

Both variants support `amd64` and `arm64`.

## Ubuntu Template

Apply the Template using:

```text
ghcr.io/boblangley/devcontainers/ubuntu:1
```

It defaults to Ubuntu 24.04 LTS (`noble`) and can select Ubuntu 26.04 LTS (`resolute`).

## Features

- `ghcr.io/boblangley/devcontainers/codex-cli:1`
- `ghcr.io/boblangley/devcontainers/claude-code-cli:1`
- `ghcr.io/boblangley/devcontainers/t3code-server:1`

## Source layout

```text
src/
├── features/
├── images/
└── templates/
```

Feature and Template releases use the official Dev Container publishing action. Ubuntu images are rebuilt weekly and on relevant changes, published with provenance and Software Bill of Materials attestations, and retained with twelve dated rollback builds per variant.
