# Projective Augmented Reality

TP réalisé à **IMT Atlantique** dans le cadre du cours d'Étienne Peillard sur la réalité augmentée projective.  
Référence : [etiennepeillard.com/teaching/lab/projective-ar](https://www.etiennepeillard.com/teaching/lab/projective-ar/)

## Description

Application de morpion en réalité augmentée projective : la caméra détecte les coups posés sur un plateau physique et le projecteur affiche le plateau de jeu en temps réel.

## Dépendances

```bash
pip install numpy==1.26.4
pip install opencv-python==4.10.0.84
pip install opencv-contrib-python==4.6.0.66
```

## Utilisation

1. Imprimer et placer les 4 marqueurs ArUco sur le plateau.
2. Lancer le programme :
   ```bash
   python main.py
   ```
3. Valider la calibration caméra/projecteur, puis jouer en posant un objet sur les cases.

## Structure

| Fichier | Rôle |
|---|---|
| `main.py` | Point d'entrée, boucle principale |
| `camera.py` | Capture vidéo |
| `projector.py` | Affichage projecteur |
| `coreAR.py` | Calibration et détection de coups |
| `ticTacToe.py` | Logique du jeu |
| `constants.py` | Paramètres globaux |
