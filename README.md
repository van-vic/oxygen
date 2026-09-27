# Oxygen Browser

Firefox soft-fork by patch-stack.
Rolling release, tracking Firefox Rapid tag-to-tag.

No divergent hard-fork. This repo is small: version pin + patches + branding + prefs + tooling. It does not contain Firefox source.

## Oxygen repos

- [oxygen](https://github.com/van-vic/oxygen) — core patches and tooling (this repo)
- [oxygen-windows](https://github.com/van-vic/oxygen-windows) — Windows packaging and installer
- `oxygen-macos` — planned
- `oxygen-linux` — planned

## Model

1. Pin official tag in `firefox_version.txt` (now `FIREFOX_156_0_1_RELEASE`).
2. Clone clean from `mozilla-firefox/firefox`.
3. Apply `patches/series` in order (Quilt style, like Helium).
4. Rebase every Rapid release. Security fixes <72h.

See `docs/philosophy.md` and `docs/transparency.md`.

## Structure
