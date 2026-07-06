# Design System — "High-Clarity" (variante Clair / light)

> ⚠️ Deux systèmes coexistent dans ce projet :
> - **`design-system.md`** = *Electric Stage* (base **sombre**, export officiel Stitch).
> - **Ce fichier** = *High-Clarity* (**clair**), l'évolution vers laquelle les 5 écrans
>   « (Clair) » ont été redessinés. Tokens extraits des données live du projet.
> Les `code.html` des écrans utilisent `class="light"` et ces rôles de couleurs clairs.

---

## Tokens (light)

```yaml
colors:
  surface: '#f9f9f9'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f3f3f3'
  surface-container: '#eeeeee'
  surface-container-high: '#e8e8e8'
  surface-container-highest: '#e2e2e2'
  on-surface: '#1a1c1c'
  on-surface-variant: '#444933'
  inverse-surface: '#2f3131'
  inverse-on-surface: '#f1f1f1'
  outline: '#747a60'
  outline-variant: '#c4c9ac'
  surface-tint: '#506600'
  primary: '#506600'
  on-primary: '#ffffff'
  primary-container: '#ccff00'      # Electric Lime
  on-primary-container: '#5b7300'
  inverse-primary: '#abd600'
  secondary: '#5f5e5e'
  on-secondary: '#ffffff'
  secondary-container: '#e5e2e1'
  tertiary: '#0046fa'               # Electric Blue
  on-tertiary: '#ffffff'
  tertiary-container: '#ebebff'
  on-tertiary-container: '#2b57ff'
  error: '#ba1a1a'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#c3f400'
  primary-fixed-dim: '#abd600'

typography:
  display-lg:        { fontFamily: Anton, fontSize: ~72px, lineHeight: 80px, letterSpacing: -0.02em }
  display-lg-mobile: { fontFamily: Anton, fontSize: 48px,  lineHeight: 48px, letterSpacing: -0.01em }
  headline-xl:       { fontFamily: Anton, fontSize: 48px,  lineHeight: 52px, letterSpacing: 0.01em }
  headline-lg:       { fontFamily: Anton, fontSize: 32px,  lineHeight: 36px, letterSpacing: 0.02em }
  body-lg:           { fontFamily: Hanken Grotesk, fontSize: 18px, lineHeight: 28px }
  body-md:           { fontFamily: Hanken Grotesk, fontSize: 16px, lineHeight: 24px }
  label-md:          { fontFamily: JetBrains Mono, fontSize: 14px, weight: 500, letterSpacing: 0.05em }
  label-sm:          { fontFamily: JetBrains Mono, fontSize: 12px, weight: 500, letterSpacing: 0.05em }

spacing: { unit: 8px, container-max: 1280px, gutter: 24px, margin-desktop: 64px, margin-mobile: 20px }
```

## Brand & Style

Esthétique **« High-Clarity »** : l'énergie brute de la scène live + la précision d'une
publication éditoriale premium. Personnalité énergique, affirmée, sophistiquée.
Style = **minimalisme à fort contraste** : espace négatif généreux, typographie audacieuse,
accents vibrants. Le mode clair apporte ouverture et rigueur ; la typo agressive garde le
côté rebelle. Résultat : une UI qui paraît à la fois haut de gamme et « loud ».

## Colors
- **Primary (Electric Lime) `#CCFF00`** — CTA à fort impact, états actifs. Texte en charbon `#121212` dessus.
- **Secondary (Deep Charcoal) `#121212`** — texte principal, icônes, structure lourde.
- **Tertiary (Electric Blue) `#0047FF`** — actions secondaires, liens, data-viz (usage parcimonieux).
- **Neutral / Surface** `#FFFFFF` (fond) et `#F8F8F8` (conteneurs subtils).

## Typography
- **Headlines → Anton** (condensée, capitales, interlignage serré).
- **Corps → Hanken Grotesk** (sans-serif nette, lisibilité maximale).
- **Data & labels → JetBrains Mono** (registre technique « stage tech »).

## Layout & Spacing
Grille fluide : 12 colonnes desktop / 4 colonnes mobile. Base 8px. Padding interne compact,
marges externes exagérées (80–120px) entre sections. Breakpoints : mobile ≤599px,
tablet 600–1023px, desktop ≥1024px.

## Elevation & Depth
Pas d'ombres : profondeur par calques translucides + contours marqués. Surfaces `#FFFFFF` /
`#F8F8F8` (ou `#CCFF00` actif). Contours 1px `#E0E0E0`. Modales : bordure 2px `#121212` +
hard-shadow décalée `4px 4px 0px`.

## Shapes
**Sharp** : border-radius 0px partout (boutons, cartes, champs). Exception : avatars
circulaires / badges (50%).

## Components
- **Buttons** — primaire : fond `#CCFF00`, texte `#121212`, rectangulaire (0px). Secondaire : bordure 2px `#121212`, sans fond.
- **Inputs** — bordure basse 1px `#E0E0E0` → 2px `#121212` au focus. Labels en JetBrains Mono 12px.
- **Cards** — bordure 1px `#E0E0E0`, angles 0px, surface blanche.
