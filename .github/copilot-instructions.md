# Content of the repository

## Devcontainer environment

- The repository is based on a devcontainer environment.

- The baseline image should be `rocker/tidyverse:4.5.0`.

- In the case of python dependencies, it should use `uv` for package management. The `pyproject.toml` file should list the dependencies needed to run whatever Python code is added.

- The image under `.devcontainer/Containerfile` should be uploaded to the GitHub Container Registry associated with this repository. And thus, all CI created by the repo should use that image.


## Examples

- This repository contains example code for Epidemiological ABMs in R and Python.

- The examples are created using quarto documents where code and markdown text is combined.

- The examples should be rather simple, avoiding featuring long scripts.

- The examples should include the minimun number of dependencies.

- All the examples should have the following structure:

  1. A metadata section indicating: "date", "author", "PR/issue" (if available).
  2. Introduction of the example.
  3. Description of the model (whaever it is). A brief mathemathical description (hopefully consistent with the other examples). If it is a network-based model or a perfect mixing model. If it is a continuous time or discrete time.
  4. The execution of the example. Run the model once (generally), and visualizing the epi curves using a simple visualization. The execution of the code should also include timing (how long it took to generate the example).
  5. References. If needed, it could include links to the original version of the example, the R/Python package used to create the example.


- The examples should be one per folder, for instance, if we have an SEIR using epiworldR, it should be under the folder `01-seir_epiworldr`, and the code as quarto readme document `01-seir_epiworldr/README.qmd`

- The repository contains a devcontainer environment. If the new example includes an R package or Python library (or other dependency) that is not included in the image file, it should be added in the `.devcontainer/Containerfile`.

- When working on agent mode, ensure that the example is executed using a container environment for its creation. Generally, you can use the `rocker/tidyverse:4.5.0` container image.

- Newly added examples should update the README.md file pointing to the folder where the example lives. For instance, `01-seir_epiworldr/`.

