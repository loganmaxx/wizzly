# Contributing to Wizzly Translations

Thank you for helping translate **Wizzly** into more languages!

This repository hosts Wizzly releases, documentation, and the official localization files under [`locales/`](locales/).

## Quick Start

1. **Fork** this repository on GitHub.
2. Read [`locales/README.md`](locales/README.md) for all formatting rules (`_meta`, `{placeholders}`, and `widgets` calendar arrays).
3. Copy [`locales/en.json`](locales/en.json) to `locales/<code>.json` (for example `locales/tr.json`, `locales/ja.json`, `locales/fr.json`, or `locales/pt-br.json`) and translate the values.
4. Validate your JSON file (make sure there are no syntax errors or trailing commas) and test it live inside Wizzly via **Settings → Interface Language → Import JSON...**.
5. Open a **Pull Request** containing only your `locales/<code>.json` file (or updated existing `.json` file).

## Don't want to use Git / Pull Requests?

You can also open a [**Translation Issue**](https://github.com/loganmaxx/wizzly/issues/new/choose) and attach or paste your translated JSON file there!

## Pull Request Checklist

- [ ] File is placed in `locales/<code>.json` with valid UTF-8 JSON syntax
- [ ] `_meta.code`, `_meta.name`, `_meta.nativeName`, `_meta.localeTag`, and `_meta.author` are filled in
- [ ] Only JSON values are translated (keys and `{placeholders}` like `{name}` or `{count}` are unchanged)
- [ ] Tested inside Wizzly via **Import JSON...**
