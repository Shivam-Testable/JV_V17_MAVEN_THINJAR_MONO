# Testable Java — `JV_V17_MAVEN_TP6152_SLIM`

Repository: [Shivam-Testable/JV_V17_MAVEN_THINJAR_MONO](https://github.com/Shivam-Testable/JV_V17_MAVEN_THINJAR_MONO)

Slim branch derived from **`JV_V17_MAVEN_THINJAR_MONO`** for **Java-only** Testable whitebox runs (TP-6152, Java derivation sheet).

## What was removed

The default branch ships four large trees used to certify tools in isolation:

- `Tool Clean (Synthetic Data)/`
- `Tool Invalid (Synthetic Data)/`
- `Tool Triggering (Synthetic Data)/`
- `Tool Triggering (Tool Github Test data)/`

Those folders add hundreds of `package.json` and Python fixtures. Testable schedules **~100+ tasks** per run on the full tree.

This branch keeps **only** the Maven monolith: `pom.xml`, `src/main/java`, `src/test/java`, `dataset.json`.

## Branches in this repo

| Branch | Use |
|--------|-----|
| `JV_V17_MAVEN_THINJAR_MONO` | Full per-tool synthetic certification |
| **`JV_V17_MAVEN_TP6152_SLIM`** | Faster Java whitebox; sheet primary tools on the domain app |

Grid cell `MVN-THIN-M` — Java **17**, Maven, thin jar, monolith. See `dataset.json` for tool pins and answer key.
