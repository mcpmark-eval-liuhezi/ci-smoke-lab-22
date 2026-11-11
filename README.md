# ci-smoke-lab-22
Throwaway sandbox for end-to-end contribution + CI smoke test

## Build artifact

This repository's CI uploads a build artifact named `demo-build` via the `.github/workflows/ci.yml` workflow, which is triggered on demand with `workflow_dispatch`. The artifact is produced by the single `build` job, which writes `demo-build.txt` and uploads it with `actions/upload-artifact@v4` under the name `demo-build`.
