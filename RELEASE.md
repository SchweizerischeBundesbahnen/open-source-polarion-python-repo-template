
# Guidelines for Releases

## Code Ownership and Automated Release Management

Releases within our project are exclusively overseen by designated code owners, as outlined in the [/ .github / CODEOWNERS](/.github/CODEOWNERS) file. Our release process is automated using the Release Please GitHub action, which is configured in [/ .github / workflows / poetry-build.yml](/.github/workflows/poetry-build.yml).

## Overview of the Workflow:

1. For the initial release, the Release Please GitHub action generates a pull request entitled "chore(main): release 1.0.0", marking the commencement of version 1.0.0. This pull request necessitates approval as required.

2. Whenever alterations are introduced to the main branch, the Release Please GitHub action dynamically creates or updates the existing pull request, titled "chore(main): release X.Y.Z", where X.Y.Z denotes the version calculated based on Git message history.


For comprehensive information, please consult the [Release Please documentation](https://github.com/googleapis/release-please).
