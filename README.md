# Flutter Format `pre-commit`

[`pre-commit`](https://pre-commit.com) hook for formatting Flutter files.

Add the following in your `.pre-commit-config.yaml`:
```yaml
- repo: https://github.com/suli1/flutter-import-sort
  rev: "master"
  hooks:
    - id: flutter-import-sort
```

You can also only include/exclude some files (defaults to only `.dart`, is a pattern):

```yaml
- repo: https://github.com/suli1/flutter-import-sort
  rev: "master"
  hooks:
    - id: flutter-import-sort
      files: lib/* # Only format source files
      exclude: lib/src/avatar.dart # Exclude the avatar widget
```

See ['import_sorter'](https://github.com/fluttercommunity/import_sorter)