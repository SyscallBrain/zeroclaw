# phone-ci

This branch only holds the workflow that builds the ZeroClaw daemon for the
owner's phone (Termux, aarch64-linux-android). The ZeroClaw code is on the
other branches:

- `master`: an exact copy of upstream (zeroclaw-labs/zeroclaw)
- `zerodroid/*`: one branch per ZeroDroid patch
- `android-master-zerodroid`: master + the patches, what the phone runs

Start it with `gh workflow run phone-build.yml -R SyscallBrain/zeroclaw`
(details at the top of `.github/workflows/phone-build.yml`).
