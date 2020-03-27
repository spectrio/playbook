# Github Packages

[Github Packages][1] provides a Github based package repository which is
namespaced and suitable for internal or external use.

## Javascript/Typescript Package Management

### Configuring Github Packages locally
Instructions how to configure **npm** or **yarn** to downloads and install
packages from Github Packages can be found [here][2].

First, the Github Packages registry needs to be referenced in the project's
`.npmrc` file.

```console
echo "registry=https://registry.npmjs.org/" >> .npmrc
echo "@spectrio:registry=https://npm.pkg.github.com/" >> .npmrc
```

Next, you need to set up your auth token in your `~/.npmrc` file
Instruction to generate a personal access token can be found [here][3].

```console
echo "//npm.pkg.github.com/:_authToken=<personal access token>" >> ~/.npmrc
```

### Configuration of package.json

Github packages requires certain fields in the `package.json` file to exactly
match the repository name in Github or the namespaced package name.

Here is the `package.json` for the [vs.vslynx-es6][4] project showing the
relevant lines for publishing.

```json
{
  "name": "@spectrio/vs.vslynx-es6",
  "repository": {
    "type": "git",
    "url": "git+ssh://git@github.com/spectrio/vs.vslynx-es6.git"
  },
  "publishConfig": {
    "registry": "https://npm.pkg.github.com/",
    "scope": "@spectrio"
  },
}
```

#### name
The name must match the package name including the **@spectrio** namespace.

```json
"name": "@spectrio/vs.vslynx-es6"
```

#### repository
The repository url must be correct
```json
"repository": {
    "type": "git",
    "url": "git+ssh://git@github.com/spectrio/vs.vslynx-es6.git"
}
```


#### publishConfig
Use this for your publish configuration.
```json
"publishConfig": {
    "registry": "https://npm.pkg.github.com/",
    "scope": "@spectrio"
}
```

[1]: https://help.github.com/en/packages/publishing-and-managing-packages/about-github-packages
[2]: https://help.github.com/en/packages/using-github-packages-with-your-projects-ecosystem/configuring-npm-for-use-with-github-packages
[3]: https://help.github.com/en/github/authenticating-to-github/creating-a-personal-access-token-for-the-command-line
[4]: https://github.com/spectrio/vs.vslynx-es6