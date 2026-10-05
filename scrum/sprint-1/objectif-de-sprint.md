# 📍Objectif de sprint

### 📍 Sprint 1 : Socle Fonctionnel & Tri de Base (MVP)

#### PB-01 — Maintien et support mécanique des pièces
* **En tant qu'** opérateur,  
* **Je veux** une structure physique stable pour fixer les composants du trieur,  
* **Afin de** garantir un alignement précis entre l'entonnoir, la zone de lecture et les réceptacles.
> **Critères d'acceptation :**
> - Toutes les pièces du modèle 3D d'origine sont imprimées et assemblées.
> - Absence de frottement bloquant la rotation des servomoteurs.

#### PB-02 — Alimentation et sécurité électrique
* **En tant qu'** opérateur,  
* **Je veux** que la carte microcontrôleur et les actionneurs soient alimentés de façon sécurisée,  
* **Afin d'** exécuter des cycles de tri en continu sans micro-coupures ni chute de tension.
> **Critères d'acceptation :**
> - La carte Nano Every alimente les deux servomoteurs et le capteur RGB sans surchauffe.
> - Le câblage électrique est validé et documenté (schéma de connexions).

#### PB-03 — Identification et distribution de base par couleur
* **En tant qu'** utilisateur,  
* **Je veux** que l'appareil identifie la couleur d'un Skittle dans la zone de mesure et positionne le bras vers le réceptacle associé,  
* **Afin d'** effectuer un tri automatique minimaliste.
> **Critères d'acceptation :**
> - Reconnaissance d'au moins 3 couleurs distinctes.
> - Acheminement correct de la friandise sans blocage sur une série de 10 Skittles.


