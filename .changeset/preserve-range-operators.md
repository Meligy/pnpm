---
"@pnpm/npm-resolver": minor
"@pnpm/manifest-utils": minor
"pnpm": minor
---

Fixed an issue where `pnpm update` would not preserve range operators (^, ~) when updating to prerelease versions. Previously, updating from `^1.0.0-beta.1` to `1.0.0-beta.2` would result in `1.0.0-beta.2` instead of `^1.0.0-beta.2`.

Now, range operators are consistently preserved for both stable and prerelease versions when running `pnpm update`.
