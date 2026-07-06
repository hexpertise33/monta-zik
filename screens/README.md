# MONTA'ZIK École de Musique — Export Stitch

Projet Stitch `12214213643286460259` · **MONTA'ZIK École de Musique** · thème *Clair (High-Clarity)*

## Contenu

```
screens/
├── site/                     ⭐ Mini-site navigable (liens entre pages câblés)
│   ├── index.html            → ouvre directement la page d'accueil
│   ├── 01_accueil.html … 05_blog.html
│   └── (double-cliquer index.html suffit — aucun serveur requis)
├── code/                     HTML/Tailwind brut de chaque écran (export officiel Stitch)
│   ├── 01_accueil.html
│   ├── 02_tarifs.html
│   ├── 03_professeurs.html
│   ├── 04_contact.html
│   └── 05_blog.html
├── images/                   Rendu PNG pleine résolution de chaque écran
│   ├── 01_accueil.png        (2560 × 7732)
│   ├── 02_tarifs.png         (2560 × 6100)
│   ├── 03_professeurs.png    (2560 × 5462)
│   ├── 04_contact.png        (2560 × 5266)
│   └── 05_blog.png           (2560 × 7230)
├── design-system.md          Design system « Electric Stage » (base sombre, export officiel)
├── design-system.high-clarity.md   Variante « High-Clarity » (claire) utilisée par les écrans
├── manifest.json             IDs, noms, dimensions, correspondances image ↔ code
├── _stitch_export_raw/       Copie brute de l'export Stitch (dossiers + screen.png par écran)
└── README.md
```

## Écrans

| # | Écran | Code | Image |
|---|-------|------|-------|
| 1 | Accueil | [01_accueil.html](code/01_accueil.html) | [01_accueil.png](images/01_accueil.png) |
| 2 | Tarifs | [02_tarifs.html](code/02_tarifs.html) | [02_tarifs.png](images/02_tarifs.png) |
| 3 | Nos Professeurs | [03_professeurs.html](code/03_professeurs.html) | [03_professeurs.png](images/03_professeurs.png) |
| 4 | Contact & Adhésion | [04_contact.html](code/04_contact.html) | [04_contact.png](images/04_contact.png) |
| 5 | Blog | [05_blog.html](code/05_blog.html) | [05_blog.png](images/05_blog.png) |
| 6 | Design System | [design-system.md](design-system.md) + [high-clarity](design-system.high-clarity.md) | — |

## Mini-site navigable (`site/`)

Version prête à parcourir : les liens de navigation (Home / Teachers / Pricing / Blog /
Membership), qui étaient tous des `href="#"` dans l'export, ont été câblés vers les bonnes
pages. **Double-clique `site/index.html`** — tout fonctionne en `file://` (liens relatifs,
assets sur CDN). Rendu vérifié dans Chrome : polices Anton/Hanken Grotesk, Tailwind, images
et design system s'affichent correctement, 0 lien cassé.

`code/` garde les fichiers bruts de l'export (liens `#` intacts) comme référence fidèle.

## Notes techniques

- **Code** : HTML + Tailwind (config des tokens intégrée), `<html class="light" lang="fr">`,
  icônes Material Symbols. Provient de l'export officiel Stitch (bouton *Exporter*).
- **Images** : téléchargées en pleine résolution (`=s0`) depuis le CDN de prévisualisation
  Stitch — plus haute définition que les `screen.png` inclus dans l'export brut.
- **Design system** : le projet contient une base sombre *Electric Stage* (`design-system.md`,
  export officiel) que les écrans « (Clair) » ont fait évoluer vers *High-Clarity* clair
  (`design-system.high-clarity.md`).
