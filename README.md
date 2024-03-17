# configs

A repository of standard config files to speed up setup of new repos

Note: Currently these files are all related to Node projects. If a package manager is related, it's probably _pnpm_.

## .github

`workflows/clean-code.yml` – A GitHub action that checks whether code is correctly formatted with prettier and aligned to the eslint config. Fails if malformatted or if eslint complains. _It doesn't automatically fix the code._

## .eslintrc.cjs

A good lint, yet not too restricting lint configuration.

Needs the following _dev dependencies_ (`pnpm add -D`):

```
@next/eslint-plugin-next
@types/eslint
@typescript-eslint/eslint-plugin
@typescript-eslint/parser
eslint
eslint-config-next
```

## .prettier.config.js

Clean code style to adhere modern standards. Tailwind config included. The following format is enforced:

- Semicolons at the end of each line
- No single quoted strings (double quotes everywhere)
- Tab width of 2 spaces
- A trailing comma where it makes sense (e.g. objects, function arguments)

Needs the following *dev dependencies* (`pnpm add -D`):

```
prettier
prettier-plugin-tailwindcss
```
