# v0.3.1

## Bug Fixes
* fix: allow scanner to terminate host compute instance (#26) (Ammar Ekbote) ([3ce8a5f](https://github.com/lacework/terraform-gcp-agentless-scanning/commit/3ce8a5fbc467219c50f4f08bae26ea9e0a5017bb))
* fix: update cloud schedule trigger to be run by orchestrate email (#37) (Ammar Ekbote) ([df07a59](https://github.com/lacework/terraform-gcp-agentless-scanning/commit/df07a599b640f3f9013359d17ee3501f018f1660))
* fix: add permision to derive machine info from monitored projects (#36) (Ammar Ekbote) ([82a035f](https://github.com/lacework/terraform-gcp-agentless-scanning/commit/82a035f0852a1954327cd94ff84d06f8b1018be9))
## Other Changes
* ci: version bump to v0.3.1-dev (Lacework)([c01c61d](https://github.com/lacework/terraform-gcp-agentless-scanning/commit/c01c61ddafc6b4c7cb93e024d22fecea721d0e61))
---
# v0.3.0

## Features
* feat: Add multi volume variable (#34) (Whitney Smith)([8102c70](https://github.com/lacework/terraform-gcp-agentless-scanning/commit/8102c7068b2c1942663188ee8b503d5097912168))
---
# v0.2.2

## Bug Fixes
* fix: avoid asking for project_id when is not needed (#24) (Salim Afiune)([e1a80ac](https://github.com/lacework/terraform-gcp-agentless-scanning/commit/e1a80ac227124da41017a0486052201962ce851a))
## Other Changes
* ci: version bump to v0.2.2-dev (Lacework)([9fb223c](https://github.com/lacework/terraform-gcp-agentless-scanning/commit/9fb223cf0260ff9176b5a53d5ce71c20c00ea887))
---
# v0.2.1

## Bug Fixes
* fix: Update tf scan frequency validation (#18) (Whitney Smith)([9277f2d](https://github.com/lacework/terraform-gcp-agentless-scanning/commit/9277f2d1cb28015083476c1e3274f43ffc5dfc02))
## Other Changes
* refactor: move custom role creation to a new file (#19) (Ammar Ekbote)([d52dfca](https://github.com/lacework/terraform-gcp-agentless-scanning/commit/d52dfca11b9064b5164448c4a4082e508071ac5f))
* chore: remove unnecessary permissions (#21) (ammarekbote)([017f38d](https://github.com/lacework/terraform-gcp-agentless-scanning/commit/017f38da476ad4969a47c576a3378c0268dfabc9))
* ci: version bump to v0.2.1-dev (Lacework)([433ea57](https://github.com/lacework/terraform-gcp-agentless-scanning/commit/433ea57ccef445d322f7df0d3ce6b8490de71608))
---
# v0.2.0

## Features
* feat: allow for custom VPC networking (#14) (Alan Nix)([8bfcdf8](https://github.com/lacework/terraform-gcp-agentless-scanning/commit/8bfcdf832ea633dfc6b3e2a4f83bab38cf23a17e))
## Other Changes
* ci: version bump to v0.1.5-dev (Lacework)([5ecb7f7](https://github.com/lacework/terraform-gcp-agentless-scanning/commit/5ecb7f7d34954ba711eba76d49b973e4a5de8ae5))
---
# v0.1.4

## Bug Fixes
* fix: removed prefix from `GCP_ORG_ID` env var (#12) (Alan Nix)([199a419](https://github.com/lacework/terraform-gcp-agentless-scanning/commit/199a419359c8920169c5477a7f82c688970024dd))
* fix: derive bucket name for regional deployments (#11) (Ammar Ekbote)([542b059](https://github.com/lacework/terraform-gcp-agentless-scanning/commit/542b0595575de333218e68cc38e7d2093c796ad8))
## Other Changes
* ci: version bump to v0.1.4-dev (Lacework)([05da03d](https://github.com/lacework/terraform-gcp-agentless-scanning/commit/05da03d9f9143479939e292a2a202c03ae0fb3e5))
---
# v0.1.3

## Bug Fixes
* fix: inherit region from Google provider configuration (#9) (Alan Nix)([e076522](https://github.com/lacework/terraform-gcp-agentless-scanning/commit/e0765222dd5eb6d4b4d74084bb286ac740a28790))
## Other Changes
* ci: version bump to v0.1.3-dev (Lacework)([28094db](https://github.com/lacework/terraform-gcp-agentless-scanning/commit/28094db5389e4c672717f1585c0e8cc89edffc9c))
---
# v0.1.2

## Bug Fixes
* fix: conditionally create the role for snapshot creation (#7) (Alan Nix)([20b23e3](https://github.com/lacework/terraform-gcp-agentless-scanning/commit/20b23e392d95ae946cb2df133d28b5b99c31b173))
## Other Changes
* ci: version bump to v0.1.2-dev (Lacework)([053f820](https://github.com/lacework/terraform-gcp-agentless-scanning/commit/053f82040a12127c30ef3f20ca74e85f0f107c87))
---
# v0.1.1

## Documentation Updates
* docs: updated examples and added project-level multi-region (#5) (Alan Nix)([67e464a](https://github.com/lacework/terraform-gcp-agentless-scanning/commit/67e464a251d734dd9b00348b21276d34a34c5f9e))
## Other Changes
* ci: version bump to v0.1.1-dev (Lacework)([1d53030](https://github.com/lacework/terraform-gcp-agentless-scanning/commit/1d530305b07941fa58462a2b65b001e8da99e596))
---
# v0.1.0

## Features
* feat: GCP agentless scanning terraform module (#1) (Alan Nix)([58638aa](https://github.com/lacework/terraform-gcp-agentless-scanning/commit/58638aa05e2e81d7ae1232f9d3be8e58f496fa94))
## Bug Fixes
* fix: updated project name in release script (#3) (Alan Nix)([52f7b0b](https://github.com/lacework/terraform-gcp-agentless-scanning/commit/52f7b0be8cb275038c0fd3b4350a55957f2185a8))
## Other Changes
* chore: update Lacework provider version to v1 (Sourcegraph)([23c4950](https://github.com/lacework/terraform-gcp-agentless-scanning/commit/23c4950d27b707cf6d5b19fe0e70f6bba441443a))
* chore: update readme (Darren Murray)([059864a](https://github.com/lacework/terraform-gcp-agentless-scanning/commit/059864a60f56a41f0899c73782a7f6b638794029))
---
