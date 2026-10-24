# How we make changes

1. Do not edit files directly on the `main` branch.
2. Create a new branch for each change, named by type and issue number, for example `docs/12-update-risk-register`.
3. Write a short, clear commit message that says what changed, for example `Update R2 mitigation (#12)`.
4. Open a pull request and ask another group member to review it.
5. The reviewer checks the change against the pull request checklist and approves it.
6. Merge the pull request. Link it to the issue so the issue closes automatically.
7. Changes to scope, schedule or budget need an approved change request issue first (see the change request template).
8. When a version is approved, the Configuration Lead creates a release tag (for example `v1.0`) and updates `CHANGELOG.md`.

Never upload passwords, keys or other secrets to this repository.
