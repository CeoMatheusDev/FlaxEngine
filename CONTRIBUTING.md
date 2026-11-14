# Contributing to this fork

Thank you for considering a contribution to the **CeoMatheusDev Flax Engine fork**.

This repository is an unofficial fork of [FlaxEngine/FlaxEngine](https://github.com/FlaxEngine/FlaxEngine). It is not the upstream project, and its issue tracker and pull requests are maintained independently.

## Before contributing

1. Read [README.md](README.md) and [LICENSE.md](LICENSE.md).
2. Make sure you have the rights to submit every part of your proposed change.
3. Check the existing issues and pull requests for duplicate work.
4. For substantial changes, open an issue or discussion first so the scope and compatibility can be agreed upon.
5. Do not submit code or content copied from projects with terms incompatible with the Flax EULA.

The Flax Engine EULA governs use of the upstream engine technology. Third-party components may have separate license terms; preserve their notices. The EULA also contains a specific assignment provision for contributions made available to Flax (section 5). A contribution to this fork is not automatically a contribution to the upstream Flax project; do not submit upstream unless you understand and accept the upstream terms.

## Licensing of contributions to this fork

Submitting a change to this repository does not, by itself, transfer copyright ownership to CeoMatheusDev or Hardion Labs.

A contribution may be designated under the [Hardion Labs Original Materials License 1.0](LICENSE-HARDION.md) only when the contributor has the necessary rights and explicitly marks or lists the relevant files as covered, as described in [docs/LICENSING.md](docs/LICENSING.md). Do not apply that license to Flax Engine code, upstream assets, or third-party material.

If you make a contribution available to the upstream Flax project (including through its GitHub network, forums, Discord, or email), review EULA section 5 first. The upstream EULA contains a contribution assignment provision. Do not submit work on behalf of another person or organization without authority to do so.

## Development workflow

1. Fork this repository within the Flax GitHub repository network where possible, or create a feature branch if you have write access.
2. Keep each change focused and use descriptive commit messages.
3. Follow the existing C++/C# formatting, naming and documentation conventions in the affected directory.
4. Avoid unrelated formatting changes and generated files.
5. Add or update tests when behavior changes.
6. Update documentation when build steps, public APIs, configuration or user-facing behavior changes.
7. Run the narrowest relevant build and tests before opening a pull request.
8. Explain the motivation, implementation, compatibility impact and validation performed in the pull request.

## Pull requests

A useful pull request includes:

- A concise summary of the problem and proposed change.
- Relevant issue links, if any.
- A description of architectural or behavioral changes.
- Build and test results, including platform and configuration.
- Notes about compatibility, migration, performance or memory implications where relevant.
- Screenshots or logs when they materially help review.

Do not claim that a pull request has been accepted by or merged into upstream Flax unless that has actually happened.

## Bug reports

When reporting a bug, include:

- Engine commit or release tag.
- Operating system, architecture and compiler/toolchain versions.
- Reproduction steps and expected versus actual behavior.
- Relevant logs, crash dumps or minimal projects, after removing secrets and private data.

## Security issues

Do not publish exploitable vulnerability details in a public issue. Follow [SECURITY.md](SECURITY.md).

## Common build checks

- Run `GenerateProjectFiles.bat` on Windows or `./GenerateProjectFiles.sh` on Linux.
- Rebuild the affected target rather than relying on stale generated files.
- Confirm Git LFS objects are present (`git lfs pull`).
- Check the repository's CI workflows for the current authoritative validation commands.

## Upstream contributions

If you intend to contribute a patch to the official Flax Engine, use the [upstream repository](https://github.com/FlaxEngine/FlaxEngine) and follow its current contribution process. Read EULA section 5 carefully: the EULA states that contributions made available to Flax are assigned to Flax, subject to the terms in that section.

## Questions

For questions about this fork, open a GitHub issue or discussion in this repository. For licensing questions about Flax Engine, contact Flax through its [official contact page](https://flaxengine.com/contact/).
