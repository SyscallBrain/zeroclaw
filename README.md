# phone-ci

Este branch é só a "oficina" do fork: tem o workflow que compila o daemon
ZeroClaw para o telemóvel (Termux, aarch64-linux-android). O código do
ZeroClaw está nos outros branches:

- `master`: cópia exacta do upstream (zeroclaw-labs/zeroclaw)
- `zerodroid/*`: um branch por patch do ZeroDroid
- `android-master-zerodroid`: master + os patches, é o que o telemóvel corre

Lançar: `gh workflow run phone-build.yml -R SyscallBrain/zeroclaw`
(detalhes no topo de `.github/workflows/phone-build.yml`).
