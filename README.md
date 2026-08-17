# project-init

Personal scaffold tool, run at the start of each new project to set up
`.private-scratch/workspace/` and `.gitignore` from templates in `templates/`.

## Development setup

Enable the tracked git hooks (runs shellcheck on staged shell scripts before commit):

```sh
git config core.hooksPath githooks
```
