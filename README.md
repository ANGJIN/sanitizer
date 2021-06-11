# Sanitizer

Analyze C# project vunlerabilities

PlanetQL provides analyzing service for c# project.  
It uses [codeQL](https://github.com/github/codeql) to analyzing project with our custom queries.  
Currently provides `Non-deterministic iteration search` query and more queries will be provided later on.

## Usage

We provide shell script automates pulling docker image and running container with planetql cli commands

setup script

```
setup.sh <c# project path> <output directory>
```

analyze script

```
analyze.sh <output directory>
```

#### Example

```zsh
$ scripts/setup.sh sample_project results

$ scripts/analyze.sh results -f --format=csv
```
