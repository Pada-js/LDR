# League des Randoms (LDR)

🎮 **League des Randoms** est un mod de jeu aléatoire inspiré de League of Legends, qui répartit automatiquement tous les champions dans les rôles classiques (Top, Jungle, Mid, ADC, Support) et génère des compositions de parties à jouer avec des règles de progression.

---

## 🔗 Accès en ligne

👉 [Jouer maintenant sur GitHub Pages](https://pada-js.github.io/LDR/)

---

## 🧠 Fonctionnement

- Tous les champions sont répartis équitablement entre les 5 rôles.
- À chaque partie, un champion aléatoire par rôle est tiré.
- En cas de victoire, ces champions sont marqués comme "gagnants" et ne peuvent plus être joués.
- En cas de défaite, chaque champion perd 1 HP et change de rôle (jamais le même deux fois).
- Si un champion tombe à 0 HP, la session est terminée.
- Le score est calculé en additionnant les HP restants des champions gagnants.

---

## 🧰 Fonctionnalités

- ✅ Système de tirage aléatoire intelligent
- ✅ Gestion de la victoire/défaite
- ✅ Score en temps réel
- ✅ Sauvegarde/import/export JSON
- ✅ Historique complet de la session (popup)
- ✅ Affichage stylisé des gagnants
- ✅ Favicon et mise en ligne GitHub Pages

---

## 📂 Utilisation

1. **Import automatique** de `champions.json` au démarrage.
2. Bouton `RESTART` : réinitialise tout.
3. Bouton `GAME` : génère une nouvelle composition.
4. Bouton `VICTOIRE` / `DEFAITE` : applique le résultat.
5. Bouton `IMPORT` / `EXPORT` : permet de charger ou sauvegarder une session.
6. Bouton `Historique de Session` : affiche les parties précédentes dans une popup.

---

## 📁 Structure du JSON

```json
{
  "champions": [
    {
      "id": 1,
      "name": "Aatrox",
      "image": "url",
      "hp": 5,
      "roles": ["top", "mid"],
      "win": false
    }
  ],
  "history": [
    {
      "id": 1,
      "win": true,
      "round": {
        "top": { ... },
        "jgl": { ... },
        "mid": { ... },
        "adc": { ... },
        "sup": { ... }
      }
    }
  ]
}
```

---

## 🧠 Idées futures

- Statistiques par champion (victoires, rôles joués)
...

---

## 👤 Auteur

Développé par **Mehdi (Pada-js)**  
💬 Projet personnel, fun et librement améliorable.

---

