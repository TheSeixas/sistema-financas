# Proposed authorization hardening

The upstream application authenticates requests, but several resource endpoints use caller-supplied IDs without an explicit ownership predicate at the service boundary.

This contribution proposes that account and transaction reads/deletes/reports be authorized against the authenticated `Usuario`, and that transaction creation verify the target account belongs to that user.

## Verification boundary

These changes were prepared and reviewed with the BDK engineering process. **They were not built or executed locally on the contributor's computer.** The repository maintainer should run `./mvnw test` and integration tests in a clean environment before merging.
