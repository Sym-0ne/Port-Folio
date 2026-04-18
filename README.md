# simonboissonnet.fr

> Portfolio personnel de **Simon Boissonnet** — étudiant BTS SIO SISR au Lycée Fulbert de Chartres,
> en recherche d'alternance pour la Licence professionnelle ASRC à partir de septembre 2026.

🔗 **Site en ligne :** <https://simonboissonnet.fr>

---

## Stack

- HTML5 sémantique (pas de framework)
- CSS3 moderne, variables CSS, grid / flex
- JavaScript vanilla (IIFE, IntersectionObserver)
- Polices : [Inter](https://rsms.me/inter/) & [JetBrains Mono](https://www.jetbrains.com/lp/mono/)
- Formulaire de contact : [Formspree](https://formspree.io)
- Hébergement : [GitHub Pages](https://pages.github.com) + domaine personnalisé via CNAME

Aucune dépendance npm, aucun build step — un simple `git push` met à jour le site.

## Structure du projet

```
.
├── index.html                                  Page d'accueil (portfolio)
├── alternance.html                             Landing recherche d'alternance
├── mentions-legales.html                       Mentions légales / RGPD
├── projets/
│   └── sport-ludique-chartres.html             Page projet technique BTS SIO SISR
├── assets/
│   ├── styles.css                              Feuille de styles partagée
│   ├── og-image.jpg                            Image Open Graph 1200×630
│   ├── favicon.svg                             Favicon monogramme SB
│   ├── photo.jpg                               Photo de profil
│   └── CV.pdf                                  CV téléchargeable
├── sitemap.xml                                 Plan du site pour les moteurs
├── robots.txt                                  Directives crawlers
├── humans.txt                                  Crédits humains
├── CNAME                                       simonboissonnet.fr
├── google80a33fc5a3186775.html                 Validation Google Search Console
├── LICENSE                                     Licence du code
└── README.md                                   Ce fichier
```

## Développement local

Le site est 100 % statique. Pour le tester en local, un simple serveur HTTP suffit :

```bash
# Python 3 (le plus simple)
python3 -m http.server 8080

# ou avec Node.js
npx http-server -p 8080

# puis ouvrir
open http://localhost:8080
```

⚠️ **Ne pas ouvrir les fichiers HTML directement depuis `file://`** — les chemins absolus (`/assets/…`)
ne résoudront pas correctement.

## Fonctionnalités SEO & accessibilité

- ✅ Données structurées JSON-LD (Person, ProfilePage, Article, BreadcrumbList)
- ✅ Open Graph + Twitter Card complets
- ✅ Sitemap XML + robots.txt
- ✅ Balise `canonical` sur chaque page
- ✅ Hiérarchie `h1` / `h2` / `h3` unique et logique
- ✅ Accessibilité WCAG 2.2 AA (skip-link, contrastes, `prefers-reduced-motion`, `focus-visible`)
- ✅ Core Web Vitals optimisés (fonts non-bloquantes, image LCP priorisée, pas de CLS)
- ✅ RGPD (pas de cookies, case de consentement formulaire, mentions légales)

## Contact

- 📧 simon.boissonnet28 [at] gmail.com
- 📞 06 45 97 19 25
- 💻 [github.com/sym-0ne](https://github.com/sym-0ne)

## Licence

Le code source de ce site est publié sous la licence indiquée dans le fichier [LICENSE](./LICENSE).
Les contenus (textes, photos, schémas) restent la propriété de Simon Boissonnet.
