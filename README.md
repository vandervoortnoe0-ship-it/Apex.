# CODEX ALPHA OS
Application opérationnelle mono-fichier (PWA) — CESS Jury 2026-2027/1.
Épreuves : FHG mardi 22/09/2026 · Sciences jeudi 24/09/2026.

## Structure
- `index.html` — TOUTE l'app : HTML + CSS + JS + données FHG/Sciences/Codex.
  Aucun autre fichier requis pour fonctionner.

## Déploiement
1. GitHub : repo → Add file → `index.html` → coller → commit.
2. Au choix :
   - Settings → Pages → branche `main` → Save → URL `*.github.io/...`
   - OU Netlify : Add new site → Import from Git → ce repo → Deploy.
3. iPhone/iPad : Safari → ouvrir l'URL → Partager → « Sur l'écran d'accueil ».

## Mise à jour
Éditer `index.html` (icône crayon) → commit → redéploiement automatique (~1 min).

## Données utilisateur
- Stockage : localStorage du navigateur (clé `codexOS_v4`).
- Sauvegarde : onglet SUIVI → boutons BACKUP / RESTORE (export JSON).
- ⚠ Vider les données Safari = perte de progression sans backup préalable.

## Contenu embarqué
- Flashcards (source : Fiches Jury 2026, PDF FHG + Sciences) :
  dates FHG · 18 outils · géo UAA 1-3 · méthode FHG (critique/synthèse) ·
  physique P5-P8 · chimie C5-C8 · biologie B4-B6 · méthode sciences (5 éléments).
- Codex stratégique : modules M1-M8 (philosophie, académique, fiscalité BE,
  corps/biohacking, ères 21-45, risques + DECISA 72h, KPI, semaine J1-J8).
- Agenda : calendrier SGS cohort 2 (Edegem) + événements personnels (travail ITM).
- Cockpit : prochaine action calculée selon jour type (examen > SGS > travail > cours).

## Versions
- v4 · 17/09/2026 : mono-fichier, design Red Aurora / liquid glass,
  fiches sciences intégrales, protocole du jour dynamique.

## Améliorations optionnelles (post-examens)
- `sw.js` : service worker pour mode hors-ligne complet.
- `apple-touch-icon.png` 180×180 : icône native iOS.
