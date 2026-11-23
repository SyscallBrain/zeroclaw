# phone-ci

This branch only holds the workflows that build for the owner's phone
(Termux, aarch64-linux-android): `phone-build.yml` (the daemon, with the
upstream sync) and `zerocode-build.yml` (the zerocode TUI). The ZeroClaw code is on the
other branches:

- `master`: an exact copy of upstream (zeroclaw-labs/zeroclaw)
- `zerodroid/*`: one branch per ZeroDroid patch
- `android-master-zerodroid`: master + the patches, what the phone runs

Start them with `gh workflow run <file> -R SyscallBrain/zeroclaw`
(details at the top of each file in `.github/workflows/`).
