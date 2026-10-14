@'
# Spécification - Devoir1 : détection de pouces levés

## But
Compter les mains qui lèvent le pouce dans une trame webcam, avec un compte stable d'une image à l'autre.

## Règles pour l'assistant (à respecter strictement)
- Modifier UNIQUEMENT `code/thumb_detector.py`.
- Ne JAMAIS modifier les tests, `detect_thumbs.py`, `emotion_detector.py` ni `check_env.py`.
- Garder la signature, les noms et l'indentation existants. Remplacer seulement le corps des fonctions à implémenter.
- Lire le docstring (Purpose, Inputs, Outputs) : c'est le contrat exact.
- Pas de print de débogage, pas de chemin en dur, pas de code mort.
- Ne pas inventer d'API : se baser sur le code et les tests réellement présents.

## Fonctions à implémenter (dans `code/thumb_detector.py`)
| Fonction | Indice | Tests |
| --- | --- | --- |
| `is_thumb_extended` | comparer les trois distances au poignet dans l'ordre MCP, IP, TIP | `test_verdict_des_cinq_mains_canoniques`, `test_pouce_leve_reste_valide_quelle_que_soit_lechelle` |
| `ThumbCounter.update` | ajouter à l'historique, publier seulement quand la fenêtre est unanime | `test_valeur_repetee_window_fois_est_publiee`, `test_valeurs_alternees_ne_publient_jamais` |

Les deux fonctions sont des feuilles du logigramme : indépendantes, dans n'importe quel ordre.

## Pièges connus
- Un seuil en coordonnées normalisées (0 à 1) dépend de la distance main-caméra : utiliser des comparaisons relatives, invariantes à l'échelle.
- Comparer deux ordonnées suppose la main verticale : une main inclinée inverse le résultat.
- Sans filtrage temporel, le compte clignote quand la détection hésite.

## Résultat attendu
- La suite `Devoir1/test` passe intégralement.
- Devant la webcam, le compte reste stable même si MediaPipe hésite une trame sur deux.
