# Container Environment

This repository uses a devcontainer environment for consistent development across different systems.

## Prerequisites

- [Docker](https://www.docker.com/get-started)
- [Visual Studio Code](https://code.visualstudio.com/)
- [Dev Containers extension](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers)

## Using the Devcontainer

1. Clone this repository:
   ```bash
   git clone https://github.com/EpiForeSITE/abm-benchmark.git
   cd abm-benchmark
   ```

2. Open in VS Code:
   ```bash
   code .
   ```

3. When prompted, click "Reopen in Container" or use the command palette (Ctrl/Cmd + Shift + P) and select "Dev Containers: Reopen in Container"

4. The devcontainer will automatically:
   - Set up the R and Python environments
   - Install necessary packages and dependencies
   - Configure VS Code extensions for R, Python, and Quarto

## Environment Details

The devcontainer is based on `rocker/tidyverse:4.5.0` and includes:

- **R environment**: Pre-configured with tidyverse and common epidemiological packages
- **Python environment**: Managed with `uv`, includes NumPy, pandas, matplotlib, and scientific computing libraries
- **Quarto**: For creating reproducible documents combining code and narrative
- **Development tools**: VS Code extensions and debugging tools

## Container Image

The repository contains a container image that has all the needed components to build and run the examples. The image is automatically built and published to the GitHub Container Registry when changes are made to the devcontainer configuration.