# Git-Flow Cheat Sheet

Git-Flow is a branching model designed to help manage the development process for large software projects with multiple contributors. It provides a structured approach to version control that keeps code organized and promotes collaboration. Below is a concise cheat sheet to help you get started with Git-Flow.

## Branches

1. **Master**
   - The mainline where all feature branches are merged.
   - Only receives stable releases.

2. **Develop**
   - The main integration branch for the next release.
   - Receives features and bug fixes for the upcoming release.

3. **Feature Branches**
   - Branch off from `develop` to add new features or enhancements.
   - Naming convention: `feature/<feature-name>`

4. **Release Branches**
   - Branch off from `develop` for a specific release cycle.
   - Merge feature branches into it, fix bugs, and prepare the release.
   - Naming convention: `release/<version-number>`

5. **Hotfix Branches**
   - Branch off from `master` to fix critical production issues in an urgent manner.
   - After fixes, merge them back into both `develop` and `master`.
   - Naming convention: `hotfix/<issue-description>`

## Commands

### Feature Branch
1. Create a feature branch:
   ```bash
   git checkout -b feature/my-new-feature develop
   ```

2. Merge a feature branch into `develop`:
   ```bash
   git checkout develop
   git merge --no-ff feature/my-new-feature
   git branch -d feature/my-new-feature
   ```

3. Push the feature branch to remote:
   ```bash
   git push origin feature/my-new-feature
   ```

### Release Branch
1. Start a release from `develop`:
   ```bash
   git checkout -b release/1.0 develop
   ```

2. Merge feature branches into the release branch:
   ```bash
   git merge --no-ff feature/my-feature
   ```

3. Finish the release and tag it:
   ```bash
   git checkout master
   git merge --no-ff release/1.0
   git tag -a v1.0 -m "Release 1.0"
   git push origin master
   git push origin master --tags
   ```

4. Merge the release branch back into `develop`:
   ```bash
   git checkout develop
   git merge --no-ff release/1.0
   git branch -d release/1.0
   git push origin develop
   ```

### Hotfix Branch
1. Start a hotfix from `master`:
   ```bash
   git checkout -b hotfix/my-hotfix master
   ```

2. Make the necessary fixes and commit them:
   ```bash
   git add .
   git commit -m "Fix critical bug"
   ```

3. Merge the hotfix into `master` and tag it:
   ```bash
   git checkout master
   git merge --no-ff hotfix/my-hotfix
   git tag -a v1.0.1 -m "Hotfix 1.0.1"
   git push origin master
   git push origin master --tags
   ```

4. Merge the hotfix into `develop`:
   ```bash
   git checkout develop
   git merge --no-ff hotfix/my-hotfix
   git branch -d hotfix/my-hotfix
   git push origin develop
   ```

## Workflow Diagram

```
+-------------------+
|                   |
|    Master         |
|                   |
+----^------------+--+
     |            |
     v            v
+----+------+  +-----------+
|      |      |           |
| Develop| Feature| Release|
|        | Branch| Branch   |
|        |       |          |
+--------+-------+----------+
```

This cheat sheet provides a quick reference to the key concepts and commands in Git-Flow. By following these guidelines, you can ensure that your development process is organized and efficient.

Happy coding!
```
