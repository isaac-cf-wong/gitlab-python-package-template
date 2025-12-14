# Python Project Template

<!--
- Pipeline
    - Update group_name
    - Update username
    - Update package_name
- Documentation
    - Update project_slug
    - Update username
    - Update package_name
- Coverage Report
    - Update group_name
    - Update package_name
- PyPI version
    - Update package_name to the name of the package.
- Python Version
    - Update package_name
- License: MIT
    - Update the License if it is not MIT.
- Security: bandit
- Zenodo DOI
    - Update ID
    - Update DOI

Remove the comment when all are done.
-->

[![Pipeline](https://gitlab.com/group_name/package_name/badges/main/pipeline.svg)](https://gitlab.com/group_name/package_name/-/pipelines)
[![Documentation](https://app.readthedocs.org/projects/project_slug/badge/?version=latest)](https://project_slug.readthedocs.io/en/latest/)
[![Coverage Report](https://gitlab.com/group_name/package_name/badges/main/coverage.svg)](https://gitlab.com/group_name/package_name/-/commits/main)
This project is a template for creating Python projects that follows PEP 621 standards. It uses pyproject.toml for configuration and Flit for building and publishing to PyPI.

To use this template on GitLab,

1. Create an empty git repository for your project.
2. Clone the template repository:

```shell
git clone git@gitlab.kuleuven.be:gwc/software/python-package-template.git <name of your package repository>
cd <name of your package repository>
```

3. Set the remote URL.

```shell
git remote set-url origin <SSH URL of your package repository>
git push
```

## Checklist

- [ ] Update the following entries in [pyproject.toml](pyproject.toml):
  - [ ] [project]
    - [ ] authors
    - [ ] description
  - [ ] [project.urls]
    - [ ] Documentation
    - [ ] Issues
    - [ ] Tracker
    - [ ] Home
    - [ ] "Release Notes"
  - [ ] [tool.flit.module]
    - [ ] name
- [ ] Update <package_name> in [.gitlab-ci.yml](.gitlab-ci.yml)
- [ ] Update [CONTRIBUTING.md](CONTRIBUTING.md)
- [ ] Update [LICENSE](LICENSE)
- [ ] Update [SECURITY.md](SECURITY.md)
- [ ] Update [SUPPORT.md](SUPPORT.md)

## Project Organization

- `.gitlab-ci.yml`: GitLab CI pipelines for building, testing, and publishing.
- `.pre-commit-config.yaml`: Pre-commit hooks configuration.
- `cliff.toml`: Configuration for generating changelogs.
- `commitlint.config.js`: Configuration for commit message linting.
- `cspell.json`: Configuration for spell checking.
- `mkdocs.yml`: Configuration for MkDocs documentation.
- `package.json`: Node.js dependencies for development tools.
- `pyproject.toml`: Python project metadata and tool configurations.
- `docs/`: Documentation source files.
- `src/`: Source code directory.
- `tests/`: Test cases.

## Getting Started

To get started, 'Use This Template' to create a new repository and start building your project in the `src` directory. Open in GitHub Codespace and run unit tests using the VS Code Test extension.
