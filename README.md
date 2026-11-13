# rhttp (fork)

This is a fork of [rhttp](https://codeberg.org/Tienisto/rhttp) by Tien Do Nam,
maintained only to carry one build fix until it lands upstream.
It is not affiliated with or endorsed by the original author.

- Upstream: <https://codeberg.org/Tienisto/rhttp> (the GitHub mirror `Tienisto/rhttp` is archived)
- Package documentation: [rhttp/README.md](rhttp/README.md)

## Changes from upstream

Based on upstream commit `39a3d766` (which includes the multi-engine Android init fix, PR #111).

| Commit | Change |
| --- | --- |
| `e5e1d85` | `rhttp/cargokit/gradle/plugin.gradle`: parse minor-versioned `compileSdkVersion`. Android Gradle Plugin 9.3+ reports API 37 as `android-37.0`, which made `substring(8) as int` throw `NumberFormatException` during Gradle configuration. |

Nothing else is modified. This fork will be retired once an upstream release contains an equivalent fix.

## License

Unchanged from upstream. See [LICENSE](LICENSE) (MIT, © Tien Do Nam) and
[rhttp/cargokit/LICENSE](rhttp/cargokit/LICENSE) (MIT or Apache-2.0, © Matej Knopp).
All original copyright and license notices are retained.
