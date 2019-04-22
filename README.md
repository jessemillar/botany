## Botany
This repo is for testing a couple theories on how my work team can use tags as part of our CI/CD pipeline to organize our builds.

## Lifecycle
1. Merge to `master`
1. The merge commit is tagged as a version (e.g. `v1.0.0`)
1. That version is deployed to dev and a smoke test is performed
1. If the smoke test passes, the version is "promoted" and tested more thoroughly in QA
1. If the QA tests pass, the version is "promoted" again and tested in QA-INT
1. If the QA-INT tests pass, the version is marked as ready to deploy
