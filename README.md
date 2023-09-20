<p align="center">
    <a href="https://www.asc-csa.gc.ca/eng/satellites/osiris-rex/">
        <img alt="Image du OSIRIS-REx | Image of OSIRIS-REx" src="https://www.asc-csa.gc.ca/images/recherche/tiles/6c7fb387-f186-4c89-9fc2-bb44ac049ac1.jpg" height="300">
        </a>
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

- [En Français](#OSIRIS-REx-Tutoriel)
- [In English](#OSIRIS-REx-Tutorial)

# OSIRIS-REx-Tutoriel

## Contexte

Le satellite OSIRIS-REx (Origins, Spectral Interpretation, Resource Identification, Security-Regolith Explorer), qui utilise le mécanisme TAGSAM (Touch-And-Go Sample Acquisition Mechanism), a été conçu pour rejoindre l'astéroïde Bennu et revenir sur Terre avec un échantillon d'astéroïde. OSIRIS-REx s'est approchée assez près de la Terre le 24 septembre 2023 pour libérer son échantillon dans l'atmosphère.<br>

L'Agence spatiale canadienne (ASC) a fourni l'altimètre laser (OLA) pour la mission d'OSIRIS-REx. L'OLA envoie des impulsions de lasers, qui sont enregistrées et traitées pour renvoyer les coordonnées et la distance des points dans un nuage de points.<br>

Cet outil s'est avéré inestimable pour fournir aux scientifiques une carte 3D précise et détaillée de la surface de Bennu. Il a permis d'analyser la forme, la pente, la rugosité et bien d'autres choses encore de Bennu. Ces informations ont ensuite été utilisées pour déterminer un site d'échantillonnage. Plusieurs sites ont été présélectionnés, et Nightingale a été choisi pour son mélange de régolithe bien préservé, son grand cratère d'échantillonnage de 140 m et sa trajectoire d'accès relativement sûre.<br>

Les nuages de points ne sont pas seulement utiles pour les applications spatiales, mais a de multiples applications sur Terre : véhicules à conduite autonome, développement de doubles numériques, sondages, imagerie, etc. Cependant, malgré ces avantages, il peut être assez difficile de travailler avec ces données en raison de leur grande quantité et leur complexité de calcul. Par conséquent, ce tutoriel a pour but de présenter au lecteur plusieurs techniques de gestion, de traitement et de visualisation des données de nuages de points.  

## Démarrage rapide

1.	Configurez un environnement virtuel ou un environnement conda avec la version suivante de python (si vous utilisez conda, remplacez le pip install ci-dessous avec conda) 
```
python = 3.7
```
2. Installer les conditions requises à partir du fichier requirments.txt
```
pip install -r requirements.txt
```
3.  Installer PDS4 Tools à partir d'un fichier zip local (plus d'informations disponibles [ici](https://sbnwiki.astro.umd.edu/wiki/Python_PDS4_Tools#Installation))
```
pip install PDS4_tools-1.3.zip
```

# OSIRIS-REx-Tutorial

## About

The Origins, Spectral Interpretation, Resource Identification, Security-Regolith Explorer (OSIRIS-REx) using the Touch-And-Go Sample Acquisition Mechanism (TAGSAM) was designed to reach the asteroid Bennu and return back to Earth with a asteroid sample. OSIRIS-REx drew close enough to Earth on September 24, 2023 to release its sample to the atmosphere.<br>

The Canadian Space Agency (CSA) contributed the Laser Altimeter (OLA) to the OSIRIS-REx satellite. The OLA sends pulses of lasers, which is recorded and processed to return the coordinates and distance of points in a point cloud.<br>

This tool was invaluable in providing scientist with an accurate and detailed 3D model of Bennu’s surface, allowing for the analysis of shape, slope, roughness, and more. This information was further used in the determination of a sample site. Several sites were shortlisted, with Nightingale being selected for its mix of well-preserved regolith, large 140m sample crater, and relatively safe access trajectory.<br>

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
3.  Install PDS4 Tools from local zipfile (more information available [here](https://sbnwiki.astro.umd.edu/wiki/Python_PDS4_Tools#Installation))
```
pip install PDS4_tools-1.3.zip
```
