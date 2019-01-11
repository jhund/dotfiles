# dotfiles

Various config dotfiles to be shared between ClearCove projects.

## .rubocop.yml

We run it with `rubocop --safe-auto-correct`.

To include this remote config file in a project, create a project `.rubocop.yml` file with the following contents:

```yml
inherit_from:
  - https://raw.githubusercontent.com/jhund/dotfiles/master/.rubocop.yml
```

To gitignore the cached remote file, add this line to your .gitignore:

```
# Ignore cached remote rubocop config file
.rubocop-*
```

See [Rubocop documentation](https://docs.rubocop.org/en/latest/configuration/#inheriting-configuration-from-a-remote-url) for more info.
