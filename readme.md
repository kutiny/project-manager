# Project Manager
This project aims to be a developer tool by opening a path in vscode or to changing current working directory in the running terminal.

## Requirements
- ```code``` as a valid command to execute vscode

## Installation

1. Download the script
    1. Using curl
        ```console=0
        curl -X GET "https://raw.githubusercontent.com/kutiny/project-manager/master/.pmrc" > ~/.pmrc
        ```
    2. Using wget
        ```console=0
        wget "https://raw.githubusercontent.com/kutiny/project-manager/master/.pmrc"
        ```
2. Add the script into your .bashrc/.zshrc
```bash
source ~/.pmrc
```

## Usage
- Open with vscode menu:
    ```console
    p
    ```
- Change directory menu:
    ```console
    p -s
    p --shell
    ```
- Add a new project:
    ```console
    p -a
    p -a my_project ~/workspace/my-project/
    p --add my_project ~/workspace/my-project/
    ```
- List projects:
    ```console
    p -l
    p --list
    ```
- Open delete menu:
    ```console
    p -d
    p --delete
    ```
- Show help:
    ```console
    p -h
    p --help
    ```
- Show version:
    ```console
    p -v
    p --version
    ```

## Known Issues

- The project name must have one word (no spaces) when using ```p -a [name] [path]``` command. Unless you modify the config file manually.
    > Config file lives in $HOME/.pm/config

## Changelog
Nothing here yet.


**Feel free to report any issues**