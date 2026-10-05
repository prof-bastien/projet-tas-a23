# Revue de sprint

# Fiche Synoptique de la Revue de Sprint (Sprint 1)

* **Durée suggérée :** 30 à 45 minutes par équipe
* **Format :** Présentation interactive devant les parties prenantes (*Product Owner*, enseignant, autres équipes)
* **Objectif central :** Démontrer l'obtention du **MVP** (*Minimum Viable Product*) — un appareil physique assemblé et capable de trier des Skittles selon le modèle original.

---

## 📋 Ordre du Jour & Contenu de la Réunion

### 1. Introduction & Objectif du Sprint (5 min)
* **Rappel de l'objectif de Sprint (*Sprint Goal*) :** 
  > *"Assembler le matériel de base, câbler le Nano Every et réaliser un tri automatique minimaliste sur quelques couleurs."*
* **Bilan du Périmètre :** Présentation des éléments du Carnet de Produit (*User Stories*) engagés lors du *Sprint Planning* (`PB-01`, `PB-02`, `PB-03`) et annonce de ce qui a été accompli versus ce qui n'a pas pu l'être.

---

### 2. Démonstration du Produit En Direct (15-20 min) — *Cœur de la revue*
> **Note :** Les étudiants effectuent une démonstration en direct sur le matériel physique (pas de simulation logicielle ni de simples diapositives).

#### 🛠️ Présentation Mécanique & Électronique
* Inspection visuelle des pièces imprimées en 3D et de l'assemblage (absence de jeu excessif, frottements du servomoteur).
* Validation du câblage sur le protoboard/breadboard relié à l'Arduino Nano Every.

![Test de la base mécanique](images/test-base-mechanic.gif)

#### ⚙️ Démonstration Fonctionnelle de Tri
* Insertion de 5 à 10 Skittles dans le réservoir d'origine.
* **Déroulement du cycle :**
  1. Alimentation de la friandise.
  2. Lecture par le capteur RGB.
  3. Orientation du bras servo vers le réceptacle correspondant.
* Mise en évidence de la précision du tri sur 2 ou 3 couleurs principales.

![Test du mécanisme de tri](images/test-base-sorting.gif)

#### ⚠️ Cas Limites / Limitations Constatées
* Démonstration en direct de l'impact de la lumière ambiante sur la lecture RGB (pour appuyer le besoin du Sprint 2).
* Démonstration du comportement lorsque le réservoir est vide ou bloqué.

---

### 3. Inspection de la « Definition of Done » (5 min)
L'équipe passe en revue la grille de conformité :
- [ ] Le code source est-il commenté ?
- [ ] Le schéma de câblage actuel est-il documenté ? *(ex. schéma simplifié ou photo annotée)*
- [ ] L'appareil fonctionne-t-il sur une alimentation autonome ?

---

### 4. Rétroaction des Parties Prenantes / Client (10 min)
Le *Product Owner* (l'enseignant ou un étudiant jouant ce rôle) donne son avis sur ce qui a été produit :
* **Validation de l'acceptation** des histoires `PB-01`, `PB-02` et `PB-03`.
* **Discussion sur les faiblesses observées** *(ex. "Le bras rate parfois l'alignement", "Le capteur confond le jaune et l'orange sous l'éclairage de la classe")*.
* **Prise de notes** pour alimenter le Carnet de Produit des Sprints 2 et 3.

---

## 📦 Livrables / Éléments requis sur la table de présentation

| Livrable | Description / État requis |
| :--- | :--- |
| **Prototype physique** | Connecté et prêt à tourner dès le début de la séance. |
| **Lot de test** | Sachet de Skittles avec les couleurs calibrées. |
| **Tableau Scrum** | À jour, montrant toutes les cartes du Sprint 1 déplacées dans la colonne `Done`. |
| **Code source** | Téléversé et fonctionnel sur la carte. |
