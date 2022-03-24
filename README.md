# chordpro_dev_env
Chordpro Development Environment for VS Code

Please adapt mount-path of your chordpro-directory in file `\.devcontainer\devcontainer.json`
It defaults to `actual-folder/../chordpro` and mounts it to `/workspaces` which is by default the VS Code working directory

  "workspaceMount": "source=${localWorkspaceFolder}/../chordpro,target=/workspace,type=bind,consistency=cached", "workspaceFolder": "/workspace",
	
