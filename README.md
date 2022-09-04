# Bash Taskfile Template

## Taskfile Creation

Download the template,

```bash
curl -so Taskfile https://raw.githubusercontent.com/acfatah/bash-taskfile/main/Taskfile.template && \
  chmod +x Taskfile
```


## Defining A Task

Create a function prefix with 'task:'. I.e,

```bash

function task:build {
  # some build task in sequence
  # build web && build mobile

  # some build task in parallel
  # build web & build mobile &
}
```

## Running A Task

Create an alias,

```bash
alias run='./Taskfile'
```

then execute `run build` to run the build command defined previously.


## Readings

* https://github.com/adriancooney/Taskfile
