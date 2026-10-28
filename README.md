# Git Branching Strategy and Workflow

This repository demonstrates a standard version control workflow using Git and GitHub, focusing on branch management, environment security, and collaborative pull requests.

## Branch Architecture

* **`main` branch:** Represents the production-ready state of the codebase.
* **`dev` branch:** Serves as the integration branch for pre-production testing.
* **`feature` branch:** Used for active development, isolation of new scripts, and updates.

## Executed Workflow

1. **Repository Initialization & Security:** 
   * Initialized a local Git repository and established the branch hierarchy.
   * Configured a `.gitignore` file to safely exclude system files, caches (`__pycache__/`), logs, and sensitive environment variables (`.env`).

2. **Application Development:**
   * Created an application script (`app.py`) on the `feature` branch to simulate a development update.
   * Verified local secrets and temporary files remained untracked by version control.

3. **Version Tagging:**
   * Applied Git tags (e.g., `v1.1.0`) to mark functional commit milestones and application states.

4. **Integration via Pull Requests:**
   * Pushed all branches and tags to the remote GitHub repository.
   * Executed a Pull Request to merge the `feature` branch into `dev` for integration.
   * Executed a final Pull Request to merge the `dev` branch into `main`, completing the deployment simulation.