# dotfiles

Various config dotfiles to be shared between ClearCove projects.

## .rubocop.yml

We run it with `rubocop --safe-auto-correct`.

To use rubocop with one of your projects follow these steps:

* Add rubocop to `development` group in your gemfile: `gem "rubocop"`
* `bundle install`
* Add this remote config file to the project. Create a file `.rubocop.yml` at the root with the following contents:

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
