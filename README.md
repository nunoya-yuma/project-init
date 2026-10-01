# project-init

Personal scaffold tool, run at the start of each new project to set up
`.private-scratch/` from templates in `templates/`.

`.private-scratch/` is kept out of git by a `.gitignore` containing `*`
placed inside it (from `templates/gitignore`), so it stays ignored even on
machines without the dotfiles global excludesFile, and the project's own
`.gitignore` is never touched.

## Development setup

Enable the tracked git hooks (runs shellcheck on staged shell scripts before commit):

```sh
git config core.hooksPath githooks
```
