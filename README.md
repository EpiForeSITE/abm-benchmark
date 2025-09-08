# ABM Benchmark: Epidemiological Agent-Based Model Examples

Welcome to the ABM Benchmark repository! This project provides a collection of epidemiological agent-based model (ABM) examples implemented in R and Python, designed for scientists in epidemiology, public health, economics, and developers working in public health research.

## 🎯 Purpose

This repository serves as a benchmark and learning resource for epidemiological modeling, featuring:

- **Simple, reproducible examples** of common epidemiological models
- **Cross-language implementations** in both R and Python
- **Consistent documentation** using Quarto documents
- **Performance benchmarking** across different modeling frameworks
- **Best practices** for epidemiological ABM development

## 🚀 Getting Started

### Prerequisites

This repository uses a devcontainer environment for consistent development across different systems. You'll need:

- [Docker](https://www.docker.com/get-started)
- [Visual Studio Code](https://code.visualstudio.com/)
- [Dev Containers extension](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers)

### Using the Devcontainer

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

### Environment Details

The devcontainer is based on `rocker/tidyverse:4.5.0` and includes:

- **R environment**: Pre-configured with tidyverse and common epidemiological packages
- **Python environment**: Managed with `uv`, includes NumPy, pandas, matplotlib, and scientific computing libraries
- **Quarto**: For creating reproducible documents combining code and narrative
- **RStudio Server**: Available on port 8787 for R development

## 📁 Repository Structure

Examples are organized in numbered folders following this structure:

```
XX-modeltype_package/
├── README.qmd          # Quarto document with the example
├── README.md          # Rendered markdown (auto-generated)
└── data/              # Input data (if needed)
```

### Current Examples

*Examples will be added here as they are contributed to the repository.*

## 📝 Example Structure

Each example follows a consistent format:

1. **Metadata**: Date, author, related PR/issue
2. **Introduction**: Brief overview of the model and its applications
3. **Model Description**: 
   - Mathematical formulation
   - Model type (network-based vs. perfect mixing)
   - Time structure (continuous vs. discrete)
4. **Implementation**: 
   - Code execution with timing information
   - Visualization of epidemiological curves
   - Performance metrics
5. **References**: Links to original implementations, packages, and literature

## 🤝 How to Contribute

We welcome contributions of new epidemiological ABM examples! Here's how to get involved:

### Adding a New Example

1. **Create an Issue**: Start by [creating an issue](https://github.com/EpiForeSITE/abm-benchmark/issues/new?template=add-example.md) proposing your new example. Use the "Add New ABM Example" template to provide details about:
   - The epidemiological model you want to implement
   - Programming language and framework
   - Model characteristics (network-based, perfect mixing, etc.)
   - Required dependencies

2. **Discussion**: The maintainers and community will discuss the proposed example, provide feedback, and help refine the implementation plan.

3. **Implementation**: Once approved, implement your example following these guidelines:
   - Create a new folder with the naming pattern: `XX-modeltype_package`
   - Write your example as a Quarto document (`README.qmd`)
   - Keep the code simple and well-documented
   - Include timing information and visualizations
   - Add any new dependencies to `.devcontainer/Containerfile`

4. **Pull Request**: Submit a pull request with your example, ensuring it follows the established structure and style.

### Contribution Guidelines

- **Simplicity**: Examples should be concise and focused on demonstrating specific modeling concepts
- **Dependencies**: Minimize external dependencies; justify any new packages
- **Documentation**: Follow the established structure for consistency
- **Testing**: Ensure your example runs successfully in the devcontainer environment
- **Performance**: Include timing information to enable benchmarking

### Areas for Contribution

We're particularly interested in examples covering:

- Different epidemiological model types (SIR, SEIR, SIRS, etc.)
- Various modeling frameworks (epiworldR, Mesa, NetworkX, etc.)
- Different population structures (networks, spatial, metapopulation)
- Public health interventions and policy scenarios
- Economic models related to health outcomes

## 📚 Resources

### Epidemiological Modeling
- [Compartmental Models in Epidemiology](https://en.wikipedia.org/wiki/Compartmental_models_in_epidemiology)
- [Agent-Based Models in Public Health](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3891442/)

### R Packages for ABM
- [epiworldR](https://github.com/UofUEpiBio/epiworldR): Fast epidemiological ABMs
- [EpiModel](https://www.epimodel.org/): Mathematical modeling of infectious disease dynamics

### Python Packages for ABM
- [Mesa](https://mesa.readthedocs.io/): Agent-based modeling framework
- [NetworkX](https://networkx.org/): Network analysis and modeling
- [EoN](https://springer-math.github.io/Mathematics-of-Epidemics-on-Networks/): Epidemics on Networks

### Quarto Documentation
- [Quarto Documentation](https://quarto.org/)
- [Quarto with R](https://quarto.org/docs/computations/r.html)
- [Quarto with Python](https://quarto.org/docs/computations/python.html)

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👥 Maintainers

This repository is maintained by the EpiForeSITE team. For questions or support, please [open an issue](https://github.com/EpiForeSITE/abm-benchmark/issues) or contact the maintainers.

## 🙏 Acknowledgments

We thank the epidemiological modeling community for their continued contributions to open science and reproducible research. Special thanks to the developers of the modeling frameworks and tools that make this benchmark possible.