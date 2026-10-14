# Plan 1 - is_thumb_extended

Fichier : `code/thumb_detector.py`. Contexte : voir spec.md.

## Instructions pour l'assistant
1. Lire le docstring complet de `is_thumb_extended` (Purpose, Inputs, Outputs).
2. Lire les tests `test_verdict_des_cinq_mains_canoniques` et `test_pouce_leve_reste_valide_quelle_que_soit_lechelle`.
3. Implémenter le corps de la fonction : calculer les distances du poignet aux points MCP, IP et TIP du pouce, et conclure « pouce étendu » selon l'ordre de ces distances (MCP, puis IP, puis TIP). Pas de seuil absolu, pas de simple comparaison d'ordonnées.
4. Ne pas toucher à `ThumbCounter.update`.
5. Lancer uniquement les tests de cette fonction et itérer jusqu'à ce qu'ils passent.

## Critère de fin
Les 2 tests de `is_thumb_extended` sont verts, sans modifier aucun test.
