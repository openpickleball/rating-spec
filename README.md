# OPEN rating spec

[![OpenSSF Scorecard](https://api.scorecard.dev/projects/github.com/openpickleball/rating-spec/badge)](https://scorecard.dev/viewer/?uri=github.com/openpickleball/rating-spec)

This repository holds the official rating spec for [OPEN](https://github.com/openpickleball), the Open Pickleball Evaluation Network, and the process for changing it.

> **Status:** No official version of the spec exists yet, and no OPEN rating is live. The [reference engine](https://github.com/openpickleball/engine) is a demonstration. Its outputs are not OPEN ratings.

## What the spec is

The spec says how an OPEN rating is calculated: the inputs it uses, the math, the parameters, and how reliability is reported. Any tool that shows an OPEN rating must conform to it. Anyone can read, fork, and build on the spec, but only the governing board changes the official version, as the [mission charter](https://github.com/openpickleball/.github/blob/main/CHARTER.md) requires.

## Layout

| Path | What it holds |
| --- | --- |
| `spec/` | The spec itself, one file per published version |
| `rfcs/` | Proposals to change the spec, numbered in order |
| `CHANGELOG.md` | Every published version and what changed |

## Changing the spec

Every change goes through a public proposal called an RFC (request for comments). See [rfcs/README.md](rfcs/README.md).

## Versions

The spec uses [Semantic Versioning](https://semver.org/):

- **Major:** a change that can move existing players' ratings, such as a new formula or a changed parameter.
- **Minor:** an addition that leaves existing ratings unchanged, such as a new optional input or a new reported statistic.
- **Patch:** a wording fix or clarification with no effect on any rating.

Each published version records the config version and config fingerprint that implement it, so any published rating can be reproduced from the match ledger.

## License

The spec and the RFCs are licensed under [CC BY 4.0](LICENSE). See [how OPEN is licensed](https://github.com/openpickleball/.github/blob/main/LICENSING.md).

## Contributing

Read the [contributing guide](https://github.com/openpickleball/.github/blob/main/CONTRIBUTING.md) first. Every commit needs a DCO sign-off (`git commit -s`). Do not put real player names, contact details, or match histories in an RFC or its evidence. Use made-up or properly de-identified data.
