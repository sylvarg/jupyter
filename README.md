# JupyterLite with the Xeus Python Kernel + Binder/Hugging Face Spaces exports

Build from the template [Xeus-Lite demo](https://github.com/jupyterlite/xeus-lite-demo).

Modifications:
- `build-environment.yml` has been updated to include `voici`
- `deploy.yml` has been modified to change the directory used by `jupyterlite` and now uses `voici build` instead of `jupyter lite build`
- `environment.yml` includes the Python packages needed for my notebooks
- the `binder` directory contains the environment required to run `voila` through [Binder](https://mybinder.org/)
- the `hf` directory contains the environment and `Dockerfile` required to run `voila` on [Hugging Face Spaces](https://huggingface.co/spaces)

Note that `voici` works correctly in this setup, but be careful with the notebooks you use:  
if they require a Python backend for interactivity (typically some uses of `ipywidgets`), you must run them with `voila`, either through [Binder](https://mybinder.org/) or via [Hugging Face Spaces](https://huggingface.co/).

---

## My notebooks using `voila` available on [Binder](https://mybinder.org/)

- Sampling and Shannon’s Theorem (analog-to-digital conversion): [![Open via MyBinder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/sylvarg/jupyter/main?urlpath=voila/render/notebooks/demo/Echantillonnage.ipynb)

- Interpolation (digital-to-analog conversion): [![Open via MyBinder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/sylvarg/jupyter/main?urlpath=voila/render/notebooks/demo/Interpolation.ipynb)

- Fourier Transform: [![Open via MyBinder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/sylvarg/jupyter/main?urlpath=voila/render/notebooks/demo/TFSD.ipynb)

---

## My notebooks using `voila` available on [Hugging Face Spaces](https://huggingface.co/spaces)

- Sampling and Shannon’s Theorem (analog-to-digital conversion): [![Open in HF Space](https://img.shields.io/badge/Launch-Open%20in%20HF%20Space-blue?logo=huggingface)](https://sylvarg-demo.hf.space/voila/render/notebooks/Echantillonnage.ipynb)

- Interpolation (digital-to-analog conversion): [![Open in HF Space](https://img.shields.io/badge/Launch-Open%20in%20HF%20Space-blue?logo=huggingface)](https://sylvarg-demo.hf.space/voila/render/notebooks/Interpolation.ipynb)

- Fourier Transform: [![Open in HF Space](https://img.shields.io/badge/Launch-Open%20in%20HF%20Space-blue?logo=huggingface)](https://sylvarg-demo.hf.space/voila/render/notebooks/TFSD.ipynb)