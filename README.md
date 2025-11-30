# Jupyterlite avec le kernel python Xeus

Template : [Xeus-Lite demo](https://github.com/jupyterlite/xeus-lite-demo).

Modifications :
- `build-environment.yml` a été modifié pour inclure `voici`
- `deploy.yml` a été modifié pour changer le dossier utilisé par `jupyerlite` et utilise `voici build` au lieu de `jupyter lite build`
- `environment.yml` inclut les paquets utiles a priori
- le répertoire `binder` contient l'environnement nécessaire pour utiliser [Binder](https://mybinder.org/) avec `voila`
- le répertoire `hf` contient l'environnement et le `Dockerfile` nécessaire pour utiliser [Hugging Space Spaces](https://huggingface.co/spaces) avec `voila`

A noter que `voici` fonctionne bien sur cette implémentation, mais attention aux notebooks utilisés : s'ils nécessitent un backend python pour l'interactivité (typiquement, certaines utilisations d'`ipywidget`), alors il fait passer sur `voila`, soit via [Binder](https://mybinder.org/), soit via [Hugging Face](https://huggingface.co/).

## Notebooks utilisant `voile` et disponibles sur [Binder](https://mybinder.org/) :
- Echantillonnage et théorème de Shannon (conversion analogique/numérique) : [![Open in Voilà via MyBinder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/sylvarg/jupyter/main?urlpath=voila/render/notebooks/demo/Echantillonnage.ipynb)
- Interpolation (conversion numérique/analogique) : [![Open in Voilà via MyBinder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/sylvarg/jupyter/main?urlpath=voila/render/notebooks/demo/Interpolation.ipynb)
- Transformée de Fourier des Signaux Discrets : [![Open in Voilà via MyBinder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/sylvarg/jupyter/main?urlpath=voila/render/notebooks/demo/TFSD.ipynb)
