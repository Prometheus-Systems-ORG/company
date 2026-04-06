# federaltrading.org → Prometheus Systems Company bridge

Pointer-only bridge derived from the current canonical consumer repo for FT.

## Source of truth

Primary upstream consumer repo:
- `https://github.com/Federal-Trading-ORG/federaltrading.org`

Primary source file in FT:
- `docs/architecture/prometheus_systems_ssot_map.md`

Referenced canonical artifacts in FT:
- `contracts/architecture/canonical/runtime_surface_matrix.yaml`
- `contracts/architecture/canonical/runtime_reconciliation.yaml`
- `contracts/architecture/canonical/dns_surface_crosswalk.yaml`
- `contracts/architecture/canonical/pve_tags_canonical_node01.yaml`
- `manifests/ssot/environments.yaml` (`prometheus-systems-via-hub.yaml`)
- `contracts/architecture/canonical/terramark_ssot_crosswalk_lock.yaml`
- `contracts/architecture/canonical/antecipagov_source_truth_lock.yaml`

## Rule

This repository stores the Prometheus-side organizing view only.

- Do not duplicate runtime secrets or `.env` from FT.
- Do not pin CT/VM credentials here.
- Changes to FT-locked references require evidence plus PR in the consumer repo first.

## Synchronization note

When FT changes shared locked fields, mirror the documentation here if and only if the change is Prometheus-facing and secret-free.
