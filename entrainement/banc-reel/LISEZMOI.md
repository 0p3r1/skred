# Annotations du banc de vidéos réelles

Position des visages sur les images du banc (`entrainement/eval-reel.mjs`). Aucune image ici : seulement des cases en pixels.
La liste des vidéos sources (Wikimedia Commons, licences libres) est sur l'issue « Réduire les carrés posés sans visage dessous ».

- `reel.json` : 5 images par extrait. Celles marquées `checked` ont été corrigées à la main : ce sont les images de nuit.
- `reel-jour-provisoire.json` : images de jour, visages pré-repérés par SCRFD-10G, pas encore corrigés. Se mesure avec `REEL=reel-jour-provisoire.json TOUT=1`.

Les 8 extraits privés du banc de nuit sont retirés. Les chiffres obtenus ne tombent donc pas exactement sur ceux de l'issue.

Utilisation : copier ces fichiers dans `<dossier des banques>/reel/`, préparer les extraits avec `entrainement/prepare-reel.py`
(il garde les annotations existantes), puis lancer `node entrainement/eval-reel.mjs <dossier des banques>`.
