# Contributing to ABM Benchmark

We welcome contributions of new epidemiological ABM examples! Here's how to get involved:

## Adding a New Example

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

## Contribution Guidelines

- **Simplicity**: Examples should be concise and focused on demonstrating specific modeling concepts
- **Dependencies**: Minimize external dependencies; justify any new packages
- **Documentation**: Follow the established structure for consistency
- **Testing**: Ensure your example runs successfully in the devcontainer environment
- **Performance**: Include timing information to enable benchmarking

## Areas for Contribution

We're particularly interested in examples covering:

- Different epidemiological model types (SIR, SEIR, SIRS, etc.)
- Various modeling frameworks (epiworldR, Mesa, NetworkX, etc.)
- Different population structures (networks, spatial, metapopulation)
- Public health interventions and policy scenarios
- Economic models related to health outcomes

## Development Environment

For detailed information about setting up the development environment, see [CONTAINERS.md](CONTAINERS.md).