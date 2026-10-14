# Plan 2 - ThumbCounter.update

Fichier : `code/thumb_detector.py`. Contexte : voir spec.md.

## Instructions pour l'assistant
1. Lire le docstring complet de `ThumbCounter.update` et le constructeur de la classe (attributs, paramètre `window`).
2. Lire les tests `test_valeur_repetee_window_fois_est_publiee` et `test_valeurs_alternees_ne_publient_jamais`.
3. Implémenter le corps : ajouter le compte à l'historique (borné à `window`), ne publier une nouvelle valeur que si l'historique est plein et que toutes ses valeurs sont identiques, sinon renvoyer la dernière valeur publiée.
4. Ne pas toucher à `is_thumb_extended`.
5. Lancer uniquement les tests de cette fonction et itérer jusqu'à ce qu'ils passent.

## Critère de fin
Les 2 tests de `ThumbCounter.update` sont verts, sans modifier aucun test.
