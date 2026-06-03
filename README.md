# Poster Animations — GitLab Pages

## Structure du projet

```
.gitlab-ci.yml         ← pipeline CI/CD (ne pas modifier)
public/
├── anim1.html         ← Animation 1 (interface_anim.gif, déjà configurée)
├── anim2.html         ← Animation 2 (placeholder à compléter)
├── anim3.html         ← Animation 3 (placeholder à compléter)
└── fig/
    ├── interface_anim.gif   ← ton GIF existant
    ├── anim2.gif            ← à ajouter
    └── anim3.gif            ← à ajouter
```

## Ajouter une animation (anim2 ou anim3)

1. Copier le fichier GIF dans `public/fig/`
2. Dans `anim2.html`, remplacer :
   ```html
   <span class="placeholder">[ fig/anim2.gif ]</span>
   ```
   par :
   ```html
   <img src="fig/anim2.gif" alt="Description de l'animation">
   ```
3. Mettre à jour le titre `<h1>` et le texte `.caption`

## URLs après déploiement

```
https://<username>.gitlab.io/<repo>/anim1.html
https://<username>.gitlab.io/<repo>/anim2.html
https://<username>.gitlab.io/<repo>/anim3.html
```

## QR codes

Générer depuis les URLs ci-dessus avec :
```bash
# Si qrencode est installé
qrencode -o qr1.png "https://<username>.gitlab.io/<repo>/anim1.html"
```
Ou via https://www.qr-code-generator.com
