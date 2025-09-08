# ABM Benchmark: Epidemiological Agent-Based Model Examples

Welcome to the ABM Benchmark repository! This project provides a collection of epidemiological agent-based model (ABM) examples implemented in R and Python, designed for scientists in epidemiology, public health, economics, and developers working in public health research.

## 🎯 Purpose

This repository serves as a benchmark and learning resource for epidemiological modeling, featuring:

- **Simple, reproducible examples** of common epidemiological models
- **Cross-language implementations** in both R and Python
- **Consistent documentation** using Quarto documents
- **Performance benchmarking** across different modeling frameworks
- **Best practices** for epidemiological ABM development

## 📁 Examples

Examples are organized in numbered folders following this structure:

```
XX-modeltype_package/
├── README.qmd          # Quarto document with the example
├── README.md          # Rendered markdown (auto-generated)
└── data/              # Input data (if needed)
```

### Current Examples

- **[01-epiworldr_seir_network/](01-epiworldr_seir_network/)** - SEIR network model using epiworldR with small-world network topology

## 🚀 Getting Started

The repository contains a container image that has all the needed components to build and run the examples. For detailed setup instructions and environment information, please see [CONTAINERS.md](CONTAINERS.md).

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

We welcome contributions of new epidemiological ABM examples! For detailed contribution guidelines, please see [CONTRIBUTE.md](CONTRIBUTE.md).

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👥 Maintainers

This repository is maintained by the EpiForeSITE team. For questions or support, please [open an issue](https://github.com/EpiForeSITE/abm-benchmark/issues) or contact the maintainers.