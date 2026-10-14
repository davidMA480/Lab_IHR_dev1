@'
# Suivi d'avancement - Devoir1

## Tests
| Test | Fonction | Statut |
| --- | --- | --- |
| test_verdict_des_cinq_mains_canoniques | is_thumb_extended | [x] |
| test_pouce_leve_reste_valide_quelle_que_soit_lechelle | is_thumb_extended | [x] |
| test_valeur_repetee_window_fois_est_publiee | ThumbCounter.update | [x] |
| test_valeurs_alternees_ne_publient_jamais | ThumbCounter.update | [x] |
| Suite complète Devoir1/test | - | [x] |

## Plans
- [x] plan1 : is_thumb_extended
- [x] plan2 : ThumbCounter.update
- [ ] Test webcam avec `code/detect_thumbs.py`
- [ ] Rapport (barème dans spec.md / énoncé)

## Journal
- is_thumb_extended : corrigée manuellement (le modèle 7b n'a pas produit l'édition)
- ThumbCounter.update : implémentée par aider (qwen2.5-coder:7b, format diff)
- Suite complète : 42 tests passés

## Problèmes rencontrés
- SyntaxError annotationlib (conflit de version Python)
- modèle 14b non installé, aider a planté (Ollama 404)
- premier essai sur la mauvaise copie du fichier (lab1 au lieu de dev1)
