# Jupyterlite with Xeus python kernel

Template taken from [Xeus-Lite demo](https://github.com/jupyterlite/xeus-lite-demo).

Modifications :
- `build-environment.yml` has been modified to include voici
- `deploy.yml` has been modified to change folder target and use `voici build` instead of `jupyter lite build`
- `environment.yml` now includes relevant packages