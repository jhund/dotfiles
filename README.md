# dotfiles

Various config dotfiles to be shared between ClearCove projects.

## .rubocop.yml

We run it with `rubocop --safe-auto-correct`.

To include this remote config file in a project, create a project `.rubocop.yml` file with the following contents:

```yml
inherit_from:
  - https://github.com/jhund/dotfiles/blob/master/.rubocop.yml
```

See [Rubocop documentation](https://docs.rubocop.org/en/latest/configuration/#inheriting-configuration-from-a-remote-url) for more info.
