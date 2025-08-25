# GitHub Actions Samples


## GitHub Actions Workflows

This repository contains several GitHub Actions workflows located in `.github/workflows/`:

### 1. `basic-workflow.yml`
**Basic Manual Workflow**

This is a simple workflow that is manually triggered. It takes user inputs (name, city, favorite color) and prints a greeting message in the Actions log.

---
You can find and modify these workflows in the `.github/workflows/` directory to suit your CI/CD needs.

### 2. `go-build-release.yml`
**Go Release Workflow**

This workflow is triggered manually (via workflow_dispatch) and builds release assets for the Go project in `src/go` for both Linux and Windows. It then uploads the built binaries as release assets to GitHub Releases for a specified tag.

Key steps:
- Checks out the code
- Sets up Go
- Builds binaries for Linux and Windows
- Uploads the binaries as release assets using the manually provided tag

asdf
