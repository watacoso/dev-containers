# dev-containers
A repository of dev container configurations for VS code.

follow this structure

```
dev-containers/
└── github.com/
    ├── project-owner-A/
    │   └── project-name-X/
    │       └── .devcontainer/
    │           ├── devcontainer.json
    │           └── Dockerfile
    └── project-owner-B/
        └── project-name-Y/
            └── .devcontainer/
                ├── devcontainer.json
                └── docker-compose.yml
```

On a machine making use of this repository, follow these steps:

- clone repository
- Open your VS Code settings.json file and add the dev.containers.repositoryConfigurationPaths setting. Point it to the directory where you cloned your configurations

```
{
    "dev.containers.repositoryConfigurationPaths": [
        "/path/to/dev-containers"
    ]
}
```

doing so will ensure that vs code will recognize a devenv to use with your project once you open it.
