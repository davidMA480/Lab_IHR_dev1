# Audit - Vérification finale

## Instructions pour l'assistant
Relire `code/thumb_detector.py` et cocher chaque point en citant la ligne concernée. Ne rien modifier sans demande explicite : signaler les écarts.

## Code
- [x] Seul code/thumb_detector.py modifié
- [x] Signatures et docstrings respectés (Purpose, Inputs, Outputs)
- [x] is_thumb_extended : aucun seuil absolu en coordonnées normalisées
- [x] is_thumb_extended : pas de simple comparaison d'ordonnées (robuste à l'inclinaison)
- [x] ThumbCounter.update : publie seulement sur fenêtre pleine et unanime
- [x] ThumbCounter.update : garde la dernière valeur publiée sinon
- [ ] Pas de print de débogage, de chemin en dur ni de code mort

## Tests
- [x] Suite Devoir1/test 100 % verte
- [x] Aucun test modifié

## Comportement réel (manuel)
- [ ] Webcam : compte stable
- [ ] Stable quand la détection hésite
- [ ] Testé à plusieurs distances et avec une main inclinée
