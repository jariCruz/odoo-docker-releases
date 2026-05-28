# odoo-docker releases

Compiled releases for [jariCruz/odoo-docker](https://github.com/jariCruz/odoo-docker) (private).

---

## Install

Run this once to install all tools and set up shell commands:

```bash
curl -fsSL https://github.com/jariCruz/odoo-docker-releases/releases/latest/download/install.sh | bash
```

Then **open a new terminal** — the commands (`new-project`, `remove-project`, `odoo-help`, etc.) will be ready to use.

> Works on macOS, Linux, and WSL.

This will:
- Download the latest `new-project` and `remove-project` binaries to `~/.local/bin`
- Add `~/.local/bin` to your `PATH`
- Register `odoo-help`, `odoo-update`, and `odoo-uninstall` as shell commands

---

## Available commands

| Command | Description |
|---|---|
| `new-project` | Interactive wizard to create a new Odoo Docker project |
| `remove-project` | Safely stop containers, remove volumes, and delete a project |
| `odoo-update` | Download the latest versions of the tools |
| `odoo-uninstall` | Remove all odoo-docker tools from your machine |
| `odoo-help` | Show all available commands |

---

## Update

```bash
odoo-update
```

Or re-run the install command — it's safe to run multiple times.

---

## Uninstall

```bash
odoo-uninstall
```

This removes the binaries from `~/.local/bin` and cleans up your `~/.bashrc` / `~/.zshrc`.

---

## Requirements

- Linux / macOS / WSL (Ubuntu recommended)
- `docker` and `docker compose` installed
- `curl` installed (pre-installed on most systems)

---

## Share with someone

Just send them the one-line install command:

```bash
curl -fsSL https://github.com/jariCruz/odoo-docker-releases/releases/latest/download/install.sh | bash && source ~/.bashrc
```
