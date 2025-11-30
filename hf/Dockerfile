FROM condaforge/mambaforge:latest

# Le container HF tourne avec l'utilisateur 1000
RUN useradd -m -u 1000 user
USER user

# Variables d'environnement de base
ENV HOME=/home/user \
    PATH=/home/user/.local/bin:$PATH

# Dossier de travail
WORKDIR $HOME/app

# Copier le contenu du Space (depuis le workflow GitHub)
COPY --chown=user . .

# Créer l'environnement conda depuis environment.yml
RUN mamba env create --prefix $HOME/env -f ./environment.yml

EXPOSE 7860
WORKDIR $HOME/app

CMD mamba run -p $HOME/env --no-capture-output voila --no-browser notebooks/