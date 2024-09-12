# ais-tuxedo-scripts

Jinja2 template maintenance scripts for [ais-tuxedo-stack](https://github.com/companieshouse/ais-tuxedo-stack) services.

<hr>

These scripts are deployed via CI/CD jobs that utilise an Ansible playbook. For more information refer to the [ais-tuxedo-stack deployment branch](https://github.com/companieshouse/ais-tuxedo-stack/tree/deployment) and [Informix Management role](https://github.com/companieshouse/ansible-collection-middleware/tree/main/roles/informix_management).

## Template scripts

This repository contains no scripts at present.

## Branching Strategy

This project uses a trunk-based branching strategy and changes merged to the `main` branch are incorporated into versioned artefacts via the [ais-tuxedo-scripts](https://github.com/companieshouse/ci-pipelines/blob/master/pipelines/ssplatform/team-infrastructure/ais-tuxedo-scripts) pipeline:

```mermaid
%%{init: { 'logLevel': 'debug', 'theme': 'default' , 'themeVariables': {
    'git0': '#4585ed',
    'git1': '#edad45'
} } }%%
gitGraph
commit
branch feature
commit
commit
commit
checkout main
merge feature tag: "1.0.0"
```

## License

This project is subject to the terms of the [MIT License](/LICENSE).
