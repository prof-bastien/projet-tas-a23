# 📦 Carnet de Produit (Product Backlog) — Trieuse de Skittles

Ce document contient l'ensemble des histoires utilisateur (*User Stories*) prioritaires pour le projet de trieuse automatique de Skittles. Les éléments sont classés par ordre de priorité.

#### PB-01 — Maintien et support mécanique des pièces
* **En tant qu'** opérateur,  
* **Je veux** une structure physique stable pour fixer les composants du trieur,  
* **Afin de** garantir un alignement précis entre l'entonnoir, la zone de lecture et les réceptacles.
> **Critères d'acceptation :**
> - Toutes les pièces du modèle 3D d'origine sont imprimées et assemblées.
> - Absence de frottement bloquant la rotation des servomoteurs.
- [x] Terminé dans le sprint numéro 1.
  
#### PB-02 — Alimentation et sécurité électrique
* **En tant qu'** opérateur,  
* **Je veux** que la carte microcontrôleur et les actionneurs soient alimentés de façon sécurisée,  
* **Afin d'** exécuter des cycles de tri en continu sans micro-coupures ni chute de tension.
> **Critères d'acceptation :**
> - La carte Nano Every alimente les deux servomoteurs et le capteur RGB sans surchauffe.
> - Le câblage électrique est validé et documenté (schéma de connexions).
- [x] Terminé dans le sprint numéro 1.

#### PB-03 — Identification et distribution de base par couleur
* **En tant qu'** utilisateur,  
* **Je veux** que l'appareil identifie la couleur d'un Skittle dans la zone de mesure et positionne le bras vers le réceptacle associé,  
* **Afin d'** effectuer un tri automatique minimaliste.
> **Critères d'acceptation :**
> - Reconnaissance d'au moins 3 couleurs distinctes.
> - Acheminement correct de la friandise sans blocage sur une série de 10 Skittles.
- [x] Terminé dans le sprint numéro 1.

#### PB-04 — Isolation lumineuse du capteur de couleur
* **En tant qu'** opérateur,  
* **Je veux** une protection optique autour de la zone de lecture RGB,  
* **Afin que** les variations de lumière ambiante de la pièce ne faussent pas la détection des couleurs.
> **Critères d'acceptation :**
> - La calibration des couleurs reste valide sous un éclairage néon puissant comme dans la quasi-obscurité.
- [ ] En cours de déveloment.

#### PB-05 — Détection du niveau de remplissage de l'entonnoir
* **En tant qu'** opérateur,  
* **Je veux** être averti lorsque le réservoir supérieur est presque vide grâce à une mesure de distance (ToF),  
* **Afin de** recharger les Skittles avant la rupture de distribution.
> **Critères d'acceptation :**
> - Mesure en temps réel de la hauteur du niveau de bonbons via le capteur ToF.
> - Détection et signalement du seuil « réservoir vide ».
- [ ] En cours de déveloment.

#### PB-06 — Contrôle de présence des bacs de réception
* **En tant qu'** opérateur,  
* **Je veux** que la machine détecte l'absence d'un bac de couleur et mette le tri en pause,  
* **Afin d'** éviter que les Skittles ne soient expulsés sur la table.
> **Critères d'acceptation :**
> - Détection de présence installée sur chaque réceptacle de couleur.
> - Arrêt immédiat du cycle de distribution lorsqu'un bac est retiré.
- [ ] En cours de déveloment.

#### PB-07 — Signalisation visuelle de l'état du système (Feux tricolores)
* **En tant qu'** utilisateur,  
* **Je veux** des témoins lumineux (DELs Rouge, Jaune, Vert) indiquant l'état de l'appareil,  
* **Afin de** connaître son statut opérationnel d'un coup d'œil.
> **Critères d'acceptation :**
> - **Vert :** Tri en cours / Système prêt.
> - **Jaune :** Niveau d'entonnoir bas.
> - **Rouge :** Entonnoir vide, bac de réception manquant ou blocage mécanique.
- [ ] En cours de déveloment.

#### PB-08 — Intégration esthétique et ergonomique des capteurs
* **En tant qu'** utilisateur,  
* **Je veux** que l'ensemble des ajouts (capteur ToF, DELs, supports de bacs) soit directement intégré au châssis 3D,  
* **Afin d'** avoir un produit propre sans fils volants ni fixations temporaires.
> **Critères d'acceptation :**
> - Pièces modifiées imprimées et ajustées sans câbles apparents non fixés.
- [ ] En cours de déveloment.

#### PB-09 — Reprise automatique et gestion des erreurs
* **En tant qu'** opérateur,  
* **Je veux** que la machine reprenne son cycle automatiquement dès qu'une erreur est corrigée,  
* **Afin d'** éviter de devoir redémarrer le système à zéro lors d'un incident.
> **Critères d'acceptation :**
> - Architecture logicielle basée sur une machine à états.
> - Reprise fluide du tri après la réinsertion d'un bac ou le réapprovisionnement de l'entonnoir.
- [ ] En cours de déveloment.


## 🛠 Exigences Transversales (Definition of Done - DoD)

Toutes les *User Stories* doivent respecter les critères suivants pour être considérées comme **Terminées** :
1. **Reproductibilité :** Les pièces imprimées en 3D doivent s'assembler sans ajustement manuel au papier de verre.
2. **Qualité du Code :** Le code est commenté, structuré de façon modulaire et poussé sur la branche `main` du dépôt Git.
3. **Performance :** Le cycle complet de tri d'une friandise ne dépasse pas **3 secondes**.
