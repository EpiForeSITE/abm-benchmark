---
name: Add New ABM Example
about: Propose a new agent-based model example for the benchmark repository
title: '[EXAMPLE] Add [Model Type] using [Package/Framework]'
labels: ['example', 'enhancement']
assignees: ''

---

## Example Description

**Brief description of the model:**
<!-- Describe what epidemiological model you want to implement (e.g., SEIR, SIR, SIRS) -->

**Programming language and package/framework:**
<!-- Specify if this will be in R or Python, and which package/framework you plan to use (e.g., epiworldR, Mesa, NetworkX) -->

**Model characteristics:**
<!-- Please check all that apply -->
- [ ] Perfect mixing model
- [ ] Network-based model
- [ ] Spatial model
- [ ] Continuous time
- [ ] Discrete time

## Implementation Details

**Mathematical description:**
<!-- Provide a brief mathematical description of the model (e.g., differential equations, transition rates) -->

**Key features to demonstrate:**
<!-- What specific aspects of the model or package do you want to showcase? -->

**Estimated complexity:**
<!-- Simple, Medium, or Complex - remember examples should be rather simple -->
- [ ] Simple (< 50 lines of code)
- [ ] Medium (50-100 lines of code)
- [ ] Complex (> 100 lines of code, needs justification)

## Dependencies

**New R packages needed:**
<!-- List any R packages not currently in the devcontainer -->

**New Python packages needed:**
<!-- List any Python packages not currently in the devcontainer -->

**System dependencies:**
<!-- Any additional system-level dependencies -->

## Additional Information

**References:**
<!-- Links to papers, documentation, or original implementations -->

**Proposed folder name:**
<!-- Suggest a name following the pattern: XX-modeltype_package (e.g., 01-seir_epiworldr) -->

**Timeline:**
<!-- When do you plan to implement this example? -->

## Checklist

Before submitting this issue, please ensure:

- [ ] I have checked that a similar example doesn't already exist
- [ ] The example targets epidemiological/public health modeling
- [ ] The dependencies are reasonable and well-maintained
- [ ] I am willing to implement this example or collaborate on its implementation