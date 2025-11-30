# Jupyterlite avec le kernel python Xeus

Template : [Xeus-Lite demo](https://github.com/jupyterlite/xeus-lite-demo).

Modifications :
- `build-environment.yml` a été modifié pour inclure `voici`
- `deploy.yml` a été modifié pour changer le dossier utilisé par `jupyerlite` et utilise `voici build` au lieu de `jupyter lite build`
- `environment.yml` inclut les paquets utiles a priori

A noter que voici fonctionne bien sur cette implémentation, mais attention aux 

## Notebooks disponibles sur mybinder:
- Animation sur l'échantillonnage et le théorème de Shannon (conversion analogique/numérique) : [![Open in Voilà via MyBinder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/sylvarg/jupyter/main?urlpath=voila/render/notebooks/demo/Echantillonnage.ipynb)
- Animation sur l'interpolation (conversion numérique/analogique) : [![Open in Voilà via MyBinder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/sylvarg/jupyter/main?urlpath=voila/render/notebooks/demo/Interpolation.ipynb)
- Animation sur la Transformée de Fourier des Signaux Discrets : [![Open in Voilà via MyBinder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/sylvarg/jupyter/main?urlpath=voila/render/notebooks/demo/TFSD.ipynb)
