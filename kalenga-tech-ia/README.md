# Kalenga | Tech & IA — Magazine tech en français

Magazine tech multi-pages construit en HTML / CSS / JavaScript simple, sans
framework ni build — hébergé gratuitement sur GitHub Pages.

Site en ligne : https://angekalenga-ai.github.io/kalenga-tech-ia/

## Contenu du dossier

```
kalenga-tech-ia/
├── index.html                  → Accueil (hero, articles à la une, domaines)
├── blog.html                   → Liste des articles avec filtres par catégorie
├── article-ia.html             → Article : Intelligence artificielle
├── article-reseaux.html        → Article : Réseaux (WiFi, box, IP, DNS, DHCP)
├── article-apprentissage.html  → Article : Coder depuis un Android
├── article-carriere.html       → Article : Premier emploi IT à Kinshasa
├── article.html                → Ancienne version courte de l'article IA (conservée)
├── a-propos.html                → Bio + parcours
├── contact.html                 → Réseaux + contact
├── css/style.css                → Tous les styles (couleurs, polices, mise en page)
├── js/script.js                 → Menu mobile, animation de fond, filtres, révélation au scroll
└── assets/                      → favicon.svg, apple-touch-icon.png, og-image.png
```

## Ajouter un nouvel article

1. Duplique un des fichiers `article-*.html` existants, renomme la copie
   (ex : `article-cybersecurite.html`)
2. Change le titre, le sommaire, le contenu et la date à l'intérieur
3. Ajoute une carte vers ce nouvel article :
   - dans `blog.html`, avec un `data-category` pour que le filtre fonctionne
   - dans la section "Articles à la une" de `index.html` si tu veux le mettre en avant
4. Mets à jour les liens "Article précédent / suivant" des articles voisins pour
   inclure le nouveau dans la boucle

## Tester le site sur ton téléphone (Acode + Termux)

```
cd ~/storage/shared/Download/kalenga-tech-ia
python -m http.server 8080
```
Puis ouvre `http://localhost:8080` dans Chrome. Modifie dans Acode, sauvegarde,
recharge la page pour voir le résultat.

## Publier une modification (Git + GitHub Pages)

```
cd ~/storage/shared/Download/kalenga-tech-ia
git add .
git commit -m "Description du changement"
git push
```
Le site se met à jour automatiquement en 1-2 minutes après le push.

## Liens déjà configurés

- Facebook : https://www.facebook.com/kalengatechAi
- X : https://x.com/angekalenga1
- Email de contact : angekalenga@gmail.com
