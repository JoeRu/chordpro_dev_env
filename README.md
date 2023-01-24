# VS Code Development Environment for Chordpro

This will enable you to work with actual Dev-Environment of [Chordpro Repository](https://github.com/ChordPro/chordpro) in an actual and modern build environment.
## Requirements
1. A working [Docker-Desktop environment](https://www.docker.com/products/docker-desktop/)
2. [Visual Studio Code](https://code.visualstudio.com/Download)

## Setup

Please clone your or the chordpro-directory.
Then clone this repository beside - so that the following structure is available
- .
- chordpro
- chordpro_dev_env

Open chordpro_dev_env folder in VS Code. You will be asked to open it in "Container" - please allow. The Dockerfile will now build all requirements for running a Perl-Dev and Debug-Server.

## .vscode - 
please copy .vscode to your chordpro directory - as it will be ignored by .gitignore it has no impact but will make your life a bit more easy.

## Adaptions

Please adapt mount-path - if choosen to be different then explained in setup - of your chordpro-directory in file `\.devcontainer\devcontainer.json`
It defaults to `actual-folder/../chordpro` and mounts it to `/workspaces` which is by default the VS Code working directory

  "workspaceMount": "source=${localWorkspaceFolder}/../chordpro,target=/workspace,type=bind,consistency=cached", "workspaceFolder": "/workspace",
	
