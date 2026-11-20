🚨 Breakra check: demo

## Breakra check: demo

### Breaking change
**Verdict: BLOCK** · bump: major
- Operation POST /orders was removed. Callers of it will receive errors. → Find and replace all calls to POST /orders.
analysis_id: sha256:31f82ae74e79415f71c30fc6e0fa961c22a3ac16f941be5d6ddccd983909cb39
Don't merge: restore POST /orders or ship it in a new major version.

### Safe change
**Verdict: SAFE** · bump: minor
analysis_id: sha256:f32d9a2fc36710002398255d53271d91cf6ccc7a208122d6afdab81058769d68
No change that may break callers (GET /customers added).