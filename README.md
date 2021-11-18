# LabVIEW_Git
API for simple Git operations written in LabVIEW

This repository contains a simple wrapper for Git command-line operations to be used in LabVIEW.
The intended use case is as part of a Continuous Integration/Deployment (CI/CD) chain, rather than for human consumption.

Note that "Git Pull" is always a combination of Fetch and Merge, so is not directly implemented. 
The collection of possible arguments becomes too large for a reasonable connector pane and so instead the Fetch and Merge operations should be used.

Only a "No-Conflicts" merge is currently implemented. 
This can be used to create "fast-forward" or non-fast-forward merge commits, but cannot handle merge conflicts.
Other implementations could in principle be added as sibling classes in future, but for CI purposes this may be unnecessary (complicated merges likely require human intervention).

# To-Do
- Package this code and produce 'releases'
- Add examples
- Improve consistency of documentation within the LabVIEW code
