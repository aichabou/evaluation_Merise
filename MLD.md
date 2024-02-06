Table : Utilisateur

- id_utilisateur (PK)
- email
- mot_de_passe
- type_utilisateur
- Photo

Table : Etudiant

- id_etudiant (PK)
- id_utilisateur (FK)
- id_session

Table : Formateur

- id_utilisateur (PK)
- id_formateur (FK)
- id_cours

Table : Session

- id_session (PK)
- nom_session
- date_debut
- date_fin

Table : Cours

- id_cours (PK)
- id_session (FK)
- nom_cours

Table : Evaluation

- id_evaluation (PK)
- id_formateur (FK)
- type_evaluation
- id_cours

Table : Evaluation_Etudiant

- id_evaluation (PK)
- id_etudiant (FK)
- note
