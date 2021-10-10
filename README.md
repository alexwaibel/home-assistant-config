<!-- markdownlint-disable MD033 MD041 -->
<br />
<div align="center">
  <h3 align="center">Home Assistant Config</h3>

  <p align="center">
    My personal home automation configuration.
    <br />
    <br />
    <a href="https://github.com/alexwaibel/home-assistant-config/issues">Report Bug</a>
    ·
    <a href="https://github.com/alexwaibel/home-assistant-config/issues">Request Feature</a>
    <br />
    <br />
  </p>

[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![GPL License][license-shield]][license-url]

</div>

<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>

<!-- markdownlint-enable MD033 -->

## About The Project

This repository contains the full configuration for my Home Assistant instance running on my home cluster. You can find more information about this in the [cluster repo](https://github.com/alexwaibel/home-cluster).

### Built With

* [Home Assistant](https://www.home-assistant.io/)
* [K3s](https://k3s.io/)
* [MQTT](https://mqtt.org/)

## Getting Started

Below are instructions for setting up your development environment. I use a container running [code-server](https://github.com/cdr/code-server) with access to the volume storing my config.

1. Access code-server via browser
1. Make changes to configuration
1. Use the Home Assistant UI to validate the config
1. Reboot Home Assistant via UI to apply changes

### Prerequisites

Install the necessary tools and pre-commit hooks so you can ensure your changes the checks.

* markdownlint

  ```sh
  npm install -g markdownlint-cli
  ```

* yamllint

  ```sh
  pip install --user yamllint
  ```

* pre-commit

  ```sh
  pip install --user pre-commit
  ```

Then install the hooks

```sh
pre-commit install
```

### Installation

1. Log in to your Home Assistant machine
1. Set your secret environment variables
1. Clone the repo

   ```sh
   git clone https://github.com/alexwaibel/home-assistant-config.git
   ```

1. Restart Home Assistant

## Contributing

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement". Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

Distributed under the GPL License. See [LICENSE.md](LICENSE.md) for more information.

## Acknowledgments

A big thanks to all the authors of the projects that make this setup possible.

* [Hyperion](https://docs.hyperion-project.org/)
* [Nabu Casa](https://www.nabucasa.com/)
* [zigbee2mqtt](https://www.zigbee2mqtt.io/)
* [zwavejs2mqtt](https://github.com/zwave-js/zwavejs2mqtt)

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[forks-shield]: https://img.shields.io/github/forks/alexwaibel/home-assistant-config.svg?style=for-the-badge
[forks-url]: https://github.com/alexwaibel/home-assistant-config/network/members
[stars-shield]: https://img.shields.io/github/stars/alexwaibel/home-assistant-config.svg?style=for-the-badge
[stars-url]: https://github.com/alexwaibel/home-assistant-config/stargazers
[issues-shield]: https://img.shields.io/github/issues/alexwaibel/home-assistant-config.svg?style=for-the-badge
[issues-url]: https://github.com/alexwaibel/home-assistant-config/issues
[license-shield]: https://img.shields.io/github/license/alexwaibel/home-assistant-config.svg?style=for-the-badge
[license-url]: https://github.com/alexwaibel/home-assistant-config/blob/main/LICENSE.txt
[product-screenshot]: images/screenshot.png
