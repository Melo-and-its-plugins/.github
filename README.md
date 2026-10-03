<a name="readme-top"></a>

<div align="center">

<!--
<img src=""
     alt="Melo logo"
     width="200"
     height="200">
-->

<h1>Melo</h1>

<p>
  Free, local and extensible music software that belongs to you.
</p>

<p>
  <a href="https://github.com/Melo-and-its-plugins/Melo">
    <img src="https://img.shields.io/badge/Main%20project-Melo-1fdcff?style=for-the-badge" alt="Melo main project">
  </a>
  <a href="https://github.com/Melo-and-its-plugins/MeloDisk">
    <img src="https://img.shields.io/badge/Official%20plugin-MeloDisk-1fdcff?style=for-the-badge" alt="MeloDisk official plugin">
  </a>
  <a href="https://github.com/Melo-and-its-plugins/Melo/blob/main/LICENSE">
    <img src="https://img.shields.io/github/license/Melo-and-its-plugins/Melo?style=for-the-badge" alt="License">
  </a>
  <img src="https://img.shields.io/badge/Rust-CE422B?style=for-the-badge&logo=rust&logoColor=white" alt="Rust">
  <img src="https://img.shields.io/badge/Open%20source-yes-success?style=for-the-badge" alt="Open source">
</p>

</div>

---

## About Melo

**Melo** is a free, local and extensible music application designed for people who want to keep control over their music library.

The project aims to offer a trustworthy alternative to ad-filled and subscription-based listening services. Melo focuses on personal music libraries: your music stays under your control, without depending on a central streaming platform.

Melo is written in **Rust** and is designed to grow through plugins.

> ⚠️ **Legal use only**  
> Melo and its plugins are intended for legal, personal and local use. Only use music that you own or are authorized to use, copy or share.

## Projects

| Repository | Description | Status |
|---|---|---|
| [Melo](https://github.com/Melo-and-its-plugins/Melo) | Main application, music library management and plugin platform | Main project |
| [MeloDisk](https://github.com/Melo-and-its-plugins/MeloDisk) | Plugin for importing audio CDs into Melo and exporting music to CDs | Official plugin |

## What Melo aims to provide

- A local music library that belongs to you
- Search and organization tools for your music
- Web radio access
- Music transfer between Melo installations
- Import and export tools for local storage media
- An extensible ecosystem of plugins

For installation instructions, development information and current project status, visit the [Melo repository](https://github.com/Melo-and-its-plugins/Melo).

## Official plugins

### MeloDisk

[MeloDisk](https://github.com/Melo-and-its-plugins/MeloDisk) helps connect physical audio CDs with your Melo library.

It aims to provide:

- Audio CD detection
- Music import from CDs into Melo
- Track metadata review before importing
- Duplicate detection and import history
- Export of selected tracks or playlists to audio CDs
- Integration into the Melo interface

> MeloDisk does not circumvent copy protection. Only use it with music and CDs you are legally allowed to copy.

## Technology

The Melo ecosystem currently relies on:

- [Rust](https://www.rust-lang.org/) for performance, memory safety and reliability
- [Iced](https://www.iced.rs/) for graphical interfaces
- [Docker](https://www.docker.com/) and Docker Compose for reproducible development environments
- GitHub Actions for automated code checks and tests

Each repository documents its own dependencies, setup instructions and supported platforms.

## Contributing

Contributions, bug reports, documentation improvements, ideas and plugins are welcome.

Please read the [Contributing Guide](../CONTRIBUTING.md) before opening an issue or Pull Request.

The general workflow is:

1. Check existing issues and Pull Requests.
2. Fork the relevant repository.
3. Create a dedicated branch.
4. Make focused changes and test them locally.
5. Open a Pull Request with a clear description.
6. Wait for review and automated checks.

## Plugin development

Melo is intended to support an ecosystem of plugins.

If you want to propose a plugin:

- Start by opening an issue in [Melo](https://github.com/Melo-and-its-plugins/Melo) to discuss your idea and integration needs.
- Do not rely on undocumented internal APIs.
- Document installation, compatibility and usage clearly.
- Add a license to your repository.
- Clearly state which Melo versions your plugin supports.
- Submit a request if you want your plugin to be listed as part of the Melo ecosystem.

The plugin API may change before the first stable release. Plugins should therefore clearly state their compatible Melo version.

## Security

Do not report security vulnerabilities through public GitHub issues.

Follow the instructions in the relevant repository’s `SECURITY.md` file. If no security policy is available yet, contact a project maintainer privately through GitHub.

## License

Each repository includes its own `LICENSE` file.

Melo and its official plugins are distributed under the **GNU Affero General Public License v3.0 (AGPL-3.0)** unless explicitly stated otherwise in the corresponding repository.

## Links

- [Melo main repository](https://github.com/Melo-and-its-plugins/Melo)
- [MeloDisk official plugin](https://github.com/Melo-and-its-plugins/MeloDisk)
- [Rust Book](https://doc.rust-lang.org/book/)
- [Iced documentation](https://docs.iced.rs/)
- [Docker documentation](https://docs.docker.com/)
- [Contributing guide](../CONTRIBUTING.md)

[Back to top](#readme-top)