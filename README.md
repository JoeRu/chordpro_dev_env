# chordpro_dev_env
Chordpro Development Environment for VS Code

Please adapt mount-path of your chordpro-directory in file '\.devcontainer\devcontainer.json'

    "mounts": [
            "source=../../chordpro,target=/workspaces,type=bind,consistency=cached"
        ],
