
> **Objectif** : Comprendre le workflow professionnel Git. En entreprise, on ne merge jamais directement dans `main` on passe par une Pull Request (PR) qui permet la revue de code par un collègue.

   
- [Dev.to](https://dev.to) — Articles DevOps et Cloud
- [Microsoft Learn](https://learn.microsoft.com) — Documentation Azure
- [GitHub Blog](https://github.blog) — Nouveautés GitHub


## Étapes simples pour ouvrir un dépôt GitHub et collaborer

1. Crée un dépôt sur GitHub et clone-le sur ton ordinateur.
   - `git clone https://github.com/username/repo.git`
   - `cd repo`
   - (si tu travailles sur un dépôt local non cloné, ajoute la remote : `git remote add origin https://github.com/username/repo.git`)

2. Si le dépôt existe déjà localement, récupère les dernières modifications.
   - `git pull origin main`

3. Crée une branche pour ton travail (`feature/nom` ou `fix/nom`).
   - `git checkout -b feature/nom`

4. Fais des changements, puis commit tes modifications avec des messages clairs.
   - `git add *`
   - `git commit -m "Message clair"

5. Pousse ta branche vers GitHub.
   - `git push -u origin feature/nom`

6. Ouvre une Pull Request pour demander la relecture.

7. Un collègue relit le code, ajoute des commentaires ou approuve.

8. Après validation, merge la PR dans `main` via GitHub.
   - `git checkout main`
   - `git pull origin main`
   - `git branch -d feature/nom`


