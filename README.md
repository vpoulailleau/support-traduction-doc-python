# Traduction de la documentation de Python

Présentation pour un atelier de traduction de la documentation officielle de
Python en français.

## Licence

CC BY-NC-SA : https://creativecommons.org/licenses/by-nc-sa/4.0/

Oui, c'est une licence non libre !

## Remarques

N'hésitez pas à ouvrir un ticket pour une remarque sur les documents.

## Installation des outils

* Installez un Ubuntu 18.04 LTS
  * En mono ou dual boot
  * Dans une machine virtuelle
  * Avec le Windows Store (seule procédure d'installation testée, car beaucoup de gens sont sous Windows − je ne suis ni sous Windows, ni sous Ubuntu…)
* Sous Windows, dans Powershell en tant qu'administrateur : `Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux`
* Démarrez Ubuntu, puis dans un terminal, exécutez les commandes suivantes
* `sudo apt update`
* `sudo apt upgrade`
  * Quand il demande `configuring libssl1.1` : sélectionnez `yes` si vous ne savez pas quoi répondre
* `sudo apt install git make python3.8 python3.8-venv python3.8-dev`
* `sudo update-alternatives --install /usr/bin/python3 python3 /usr/bin/python3.6 1`
* `sudo update-alternatives --install /usr/bin/python3 python3 /usr/bin/python3.8 2`
* Installez `poedit`
  * Sous Windows https://download.poedit.net/Poedit-2.2.4-setup.exe
  * Sous Linux (pas installé avec le Windows Store) : `sudo apt install poedit`
  * Configurez `poedit` comme mentionné dans les planches
* Allez dans votre dossier « Mes documents »
  * Dans un Ubuntu du Windows Store : `cd /mnt/c/Users/VOTRE_LOGIN/Documents/`
  * Dans un Ubuntu normal : `cd`
* `mkdir traduction_python_docs`
* Faire votre fork dans GitHub
* `git clone https://github.com/VOTRE_LOGIN/python-docs-fr.git`
* `cd python-docs-fr/`
* `git remote add upstream https://github.com/python/python-docs-fr.git`
* `git fetch upstream`
* `make todo`
* `source venv/bin/activate`
* fetch + création de branche
