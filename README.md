# Matrix Build with Artifacts

This repository demonstrates GitHub Actions matrix builds with artifact management.

## Workflow Features

- **Matrix Strategy**: Builds across multiple OS and Python version combinations
- **Parallel Execution**: All matrix variants run simultaneously  
- **Artifact Management**: Each job generates and uploads unique build artifacts
- **Artifact Naming**: Uses prefix `build-c391963-<variant>` as required
- **Step Identifier**: Includes the required `matrix-c391963` step identifier

## Matrix Variants

The workflow builds for these combinations:
- Ubuntu + Python 3.9
- Ubuntu + Python 3.10  
- Ubuntu + Python 3.11
- Windows + Python 3.10
- macOS + Python 3.11

## Artifacts

Each matrix job generates:
- Build information file
- Build log output  
- Platform metadata in JSON format
- Combined artifact uploaded with proper naming

## Validation Requirements Met

✅ At least 3 successful matrix jobs  
✅ At least 3 artifacts uploaded with prefix `build-c391963`  
✅ All artifacts contain actual content (non-empty)  
✅ Step includes identifier `matrix-c391963`  
✅ Repository contains README.md with email address

## Contact

Email: 23f3003311@ds.study.iitm.ac.in

---

*This workflow demonstrates advanced CI/CD practices with GitHub Actions matrix builds and artifact management.*
