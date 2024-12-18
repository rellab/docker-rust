# docker-rust

A docker container for Rust

## Usage

## Usage with VSCode

```json
{
    "name": "Rust Development Container",
    "image": "rust:bullseye",
    "customizations": {
        "vscode": {
            "extensions": [
                "rust-lang.rust-analyzer"
            ],
            "settings": {
                "terminal.integrated.shell.linux": "/bin/bash"
            }
        }
    },
    "runArgs": [
        "--privileged"
    ],
    "workspaceMount": "source=${localWorkspaceFolder},target=/workspace,type=bind,consistency=cached",
    "workspaceFolder": "/workspace"    
}
```
