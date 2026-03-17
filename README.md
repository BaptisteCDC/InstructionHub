# Test Awesome Coding Assistant

Ce repository contient une base de personnalisation GitHub Copilot pour VS Code:

- Instructions globales projet
- Instructions spécialisées par domaine
- Skill réutilisable pour les tâches fréquentes

## Structure

- `.github/copilot-instructions.md`: règles globales Copilot pour le projet
- `.github/instructions/*.instructions.md`: instructions ciblées avec `applyTo`
- `.github/skills/create-feature-spec/SKILL.md`: skill de génération de spécification fonctionnelle
- `.github/skills/create-feature-spec/templates/feature-spec-template.md`: modèle utilisé par le skill

## Utilisation

1. Ouvre Copilot Chat dans VS Code.
2. Demande une tâche de code dans ce repo: les instructions globales seront prises en compte automatiquement.
3. Pour exploiter le skill, demande par exemple:
   - "Crée une spec de feature pour l'authentification SSO"

## Notes

- Les instructions de `.github/instructions/` sont appliquées selon leurs motifs `applyTo`.
- Le skill est déclenché selon sa description et les mots-clés présents dans la demande.
