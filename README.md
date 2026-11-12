# pramadani-osm-modules

Logos module catalog for [logos-osm-distribution](https://github.com/pramadanif/logos-osm-distribution)
(LP-0018: OpenStreetMap snapshots registered on the Logos Execution Zone and distributed through
Logos Storage). Made from [`logos-co/logos-modules-release-base`](https://github.com/logos-co/logos-modules-release-base);
its original README is kept as `README-release-base.md`.

Add this catalog to the package manager (Basecamp or `lgpd`):

    https://raw.githubusercontent.com/pramadanif/pramadani-osm-modules/main/logos-repo.json

| Module | Type | Source folder |
|--------|------|---------------|
| `pramadani_osm_sdk` | core | `basecamp/osm-sdk` |
| `pramadani_osm_distribution` | core | `basecamp/osm-distribution` |
| `pramadani_osm_app` | Basecamp app | `basecamp/osm-app` |
| `pramadani_osm_consumer_module` | template, core | `examples/consumer-module` |
| `pramadani_osm_consumer_app` | template, app | `examples/distribution-consumer-app` |

All five come from one submodule, `submodules/logos-osm-distribution`, pinned to the commit that
is released; `modules.txt` lists the module folders. Variants: `darwin-arm64`, `linux-amd64`.

Release: Actions → **Release all modules** (or one **Release pramadani_osm_…**). To publish a new
version, move the submodule to the new commit, bump `version` in that module's `metadata.json`,
and run the workflow again.
