<p align="center">
    <a href="https://www.asc-csa.gc.ca/eng/satellites/osiris-rex/">
   <img src="https://www.asc-csa.gc.ca/images/recherche/tiles/6c7fb387-f186-4c89-9fc2-bb44ac049ac1.jpg" alt="Image du OSIRIS-REx | Image of OSIRIS-REx" height=300>
    </a>
    <br> Crédit d'image | Image credit: <a href="https://www.asc-csa.gc.ca/eng/satellites/osiris-rex/">ASC-CSA</a>
</p>

<p align="center">
    <a href="#stars">
        <img alt="Étoiles sur GitHub | GitHub Repo stars" src="https://img.shields.io/github/stars/asc-csa/OSIRIS-REx-Tutorial">
    </a>
    <a href="#watchers">
        <img alt="Spectateurs sur Github | GitHub watchers" src="https://img.shields.io/github/watchers/asc-csa/OSIRIS-REx-Tutorial">
    </a>
    <a href="https://github.com/asc-csa/OSIRIS-REx-Tutorial/commits/main">
        <img alt="Dernier commit sur GitHub | GitHub last commit" src="https://img.shields.io/github/last-commit/asc-csa/OSIRIS-REx-Tutorial">
    </a>
    <a href="https://github.com/asc-csa/OSIRIS-REx-Tutorial/graphs/contributors">
        <img alt="Contributeurs sur GitHub | GitHub contributors" src="https://img.shields.io/github/contributors/asc-csa/OSIRIS-REx-Tutorial">
    </a>
    <a href="https://twitter.com/intent/follow?screen_name=csa_asc">
        <img alt="Suivre sur Twitter | Twitter Follow" src="https://img.shields.io/twitter/follow/csa_asc?style=social">
    </a>
</p>

---

<h3 align="center">
  <a href="#titre-du-projet">Français</a> |
  <a href="#project-title">English (follows)</a>
</h3>

---

<a id="titre-du-projet"></a>
# OSIRIS-REx - Tutoriel

> **Description brève :**
> Ce tutoriel présente des techniques de gestion, de traitement et de visualisation des nuages de points issus de la mission OSIRIS-REx.

## À propos

**OSIRIS-REx - Tutoriel** est un tutoriel Jupyter Notebook qui guide les utilisateurs à travers les techniques de gestion, de traitement et de visualisation des nuages de points issus de la mission OSIRIS-REx. Il couvre :

- Gestion et traitement des données de nuages de points 3D
- Visualisation des données de l'altimètre laser (OLA)
- Techniques d'analyse de surface d'astéroïdes
- Applications des nuages de points en science planétaire

Le vaisseau spatial OSIRIS-REx a été conçu pour rejoindre l'astéroïde Bennu et revenir sur Terre avec un échantillon. L'Agence spatiale canadienne (ASC) a fourni l'altimètre laser (OLA) qui a permis de créer une carte 3D précise de la surface de Bennu.

*Ce tutoriel est fourni à des fins pédagogiques et expérimentales.*  

## Prérequis

- Python 3.7
- Jupyter Notebook ou Jupyter Lab
- Connexion Internet (pour le téléchargement des données)
- PDS4 Tools pour le traitement des données OSIRIS-REx

## Démarrage rapide

1. 📦 **Cloner le dépôt**
   ```bash
   git clone https://github.com/asc-csa/OSIRIS-REx-Tutorial.git
   cd OSIRIS-REx-Tutorial
   ```
2. 🐍 **Créer un environnement**
   ```bash
   # Avec virtualenv
   python -m venv env
   source env/bin/activate

   # Ou avec conda
   conda create -n osiris_env python=3.7
   conda activate osiris_env
   ```
3. 📥 **Installer les dépendances**
   ```bash
   pip install -r requirements.txt
   pip install PDS4_tools-1.3.zip
   ```
4. 🚀 **Lancer le tutoriel**
   ```bash
   jupyter notebook
   ```

> **Remarque :** PDS4 Tools est nécessaire pour traiter les données OSIRIS-REx. Plus d'informations [ici](https://sbnwiki.astro.umd.edu/wiki/Python_PDS4_Tools#Installation).

## Licence

Ce projet est sous une licence MIT modifiée – voir le fichier [LICENSE](https://github.com/asc-csa/OSIRIS-REx-Tutorial/blob/main/LICENSE.txt) pour plus de détails.

---

<h3 align="center">
  <a href="#project-title">English </a> |
  <a href="#titre-du-projet">Français (précède)</a>
</h3>

---

<a id="project-title"></a>
# OSIRIS-REx Tutorial

> **Brief description:**
> This tutorial introduces techniques for managing, processing, and visualizing point cloud data from the OSIRIS-REx mission.

# OSIRIS-REx-Tutorial

## About

The Origins, Spectral Interpretation, Resource Identification, Security-Regolith Explorer (OSIRIS-REx) using the Touch-And-Go Sample Acquisition Mechanism (TAGSAM) was designed to reach the asteroid Bennu and return back to Earth with an asteroid sample. OSIRIS-REx drew close enough to Earth on September 24, 2023 to release its sample to the atmosphere.<br>

The Canadian Space Agency (CSA) contributed the Laser Altimeter (OLA) to the OSIRIS-REx spacecraft. The OLA sends pulses of lasers, which is recorded and processed to return the coordinates and distance of points in a point cloud.<br>

This tool was invaluable in providing scientists with an accurate and detailed 3D model of Bennu’s surface, allowing for the analysis of shape, slope, roughness, and more. This information was further used in the determination of a sample site. Several sites were shortlisted, with Nightingale being selected for its mix of well-preserved regolith, large 140m sample crater, and relatively safe access trajectory.<br>

Point cloud data not only provides benefits for space-based applications, but has many applications here on Earth, from self-driving vehicles, digital twin development, surveys, imaging and more. Despite these benefits, this data can still be quite difficult to work with due to its large size and computational complexity. Therefore, this tutorial seeks to introduce the reader to several techniques in the management, processing and visualization of point cloud data.  

## Quick Start

1.	Setup a virtual environment or conda environment with the following version of python (if using conda replace the below pip install with conda)
```
python = 3.7
```
2.  Install requirements from the requirments.txt file
```
pip install -r requirements.txt
```
3.  Install PDS4 Tools from a local zipfile (more information available [here](https://sbnwiki.astro.umd.edu/wiki/Python_PDS4_Tools#Installation))
   ```
   pip install PDS4_tools-1.3.zip
   ```

## License

This project is licensed under a modified MIT license - see the [LICENSE](https://github.com/asc-csa/OSIRIS-REx-Tutorial/blob/main/LICENSE.txt) file for details.
