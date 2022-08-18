<div id="top" />

<br />
<div align="center">
  <a href="https://github.com/trophoria">
    <img src="https://github.com/trophoria/.github/blob/main/brand/brand.png" width="500" alt="trophoria logo" />
  </a>

  <br />
  <br />

  <p align="center">
    Linting configurations for trophoria's dart/flutter and typescript projects.
    <br />
    <a href="https://github.com/trophoria/trophoria-lints/"><strong>« Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://github.com/trophoria/trophoria-lints/issues/new?template=bug_report.md">Report Bug</a>
    ·
    <a href="https://github.com/trophoria/trophoria-lints/issues/new?template=feature_request.md">Request Feature</a>
  </p>

  <p align="center">
  	<a href="https://github.com/trophoria/trophoria-lints/blob/main/LICENSE" title="license">
        <img src="https://img.shields.io/github/license/trophoria/trophoria-lints?style=for-the-badge" alt="license" />
    </a>
  </p>
</div>

<details>
  <summary>Table of Contents</summary>
  <ol>
    <li><a href="#👋-getting-started">👋 Getting Started</a></li>
    <li><a href="#👥-contributing">👥 Contributing</a></li>
    <li><a href="#🪲-issue-reporting">🪲 Issue Reporting</a></li>
    <li><a href="#🔓-license">🔓 License</a></li>
    <li><a href="#💌-contact">💌 Contact</a></li>
  </ol>
</details>


## 👋 Getting started

Welcome to trophoria! This repository contains an ansible playbook which is used to easily setup a secured remote linux server to run a whole trophoria backend.

If you want to contribute to our community projects, we advice you to fist read through our [wiki pages](https://github.com/trophoria/.github/wiki). If you for example want to learn, how we set up our development environment, you can read our [Development setup](https://github.com/trophoria/.github/wiki/2-Development-setup). This repository itself contains more useful information like pull request templates, security guidelines and so on. Make sure to read those too!

This repository contains our linting configurations we use in our typescript and flutter projects. 

### Typescript

Install both linting packages for `eslint` and `prettier` via yarn:

```bash
yarn add -D @trophoria/eslint-config @trophoria/prettier
```

Now add the following configuration to your `package.json` file:

```json
{
  "prettier": "@trophoria/prettier-config",
  "eslintConfig": {
    "extends": [ "@trophoria/eslint-config" ]
  }
}

```

### Flutter

Add the linting package to your `pubspec.yaml` file:

```yaml
dev_dependencies:
  trophoria_lints:
    git: 
      url: https://github.com/trophoria/trophoria-lints.git
      path: trophoria-flutter
```

Now you can include the config in your `analysis_options.yaml` file:

```yaml
include: package:trophoria_lints/lints.yaml
```

<p align="right">(<a href="#top">back to top</a>)</p>

## 👥 Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this project better, please fork the repo and create a pull request. Don't forget to give the project a star! Thanks again! But before you get started, please see the following pages first:

- [Code of Conduct](.github/CODE_OF_CONDUCT.md)
- [Contributing Guidelines](.github/CONTRIBUTING.md)

You can also take a look at the already mentioned wiki pages to find a few guides on how to work with the repository technologies and so on. We also included a pull request template which includes a pretty large checklist of things, you should already fulfill before creating a merge request, to keep the review time as small as possible! 

<p align="right">(<a href="#top">back to top</a>)</p>

## 🪲 Issue Reporting

If you have found a bug or if you have a feature request, please report them at this repository issues section. For other related questions/support please use the official [discord server](https://discord.gg/qWPyFWkff6). More information about issue reporting contributing are found in the [Contributing](./.github/CONTRIBUTING.md) guidelines.

<p align="right">(<a href="#top">back to top</a>)</p>

## 🔓 License

All of our software is distributed under the MIT License. See the [LICENSE](./LICENSE) file for more information.

<p align="right">(<a href="#top">back to top</a>)</p>

## 💌 Contact

If you are interested in connecting with us, don't hesitate to do so. Either write us an email to [trophoria@gmail.com](mailto:trophoria@gmail.com) or join our [community discord ](https://discord.gg/qWPyFWkff6).

<p align="right">(<a href="#top">back to top</a>)</p>
