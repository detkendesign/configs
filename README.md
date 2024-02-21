# configs
A repository of standard config files to speed up setup of new repos

Note: Currently these files are all related to Node projects. If a package manager is related, it's probably *pnpm*.

## .github

`workflows/clean-code.yml` – A GitHub action that checks whether code is correctly formatted with prettier and aligned to the eslint config. Fails if malformatted or if eslint complains. *It doesn't automatically fix the code.*

