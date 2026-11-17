# MVLink auto-update builds

Public Sparkle auto-update feed for MVLink, the Mac client of the private [MVRDP](https://github.com/superbam/MVRDP) project.

Nothing here is hand-edited: the `dev` pre-release (only `MVLink.app.zip` + `appcast.xml`) is published automatically by that repo's CI on every push to main. Binaries are Developer ID signed, notarized, and EdDSA-signed by the private pipeline; MVLink only accepts updates that verify against the public key baked into it, so an attacker who could write this repo still could not forge an update.
