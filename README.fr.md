# IrsanAI · LRP v1.3

> 🌍 **Lisez ce README dans votre langue:**
> [🇬🇧 English](README.en.md) | [🇩🇪 Deutsch](README.md) | [🇪🇸 Español](README.es.md) | [🇮🇹 Italiano](README.it.md) | [🇧🇦 Bosanski](README.bs.md) | [🇷🇺 Русский](README.ru.md) | [🇨🇳 中文](README.zh.md) | [🇫🇷 Français](README.fr.md) | [🇧🇷 Português (BR)](README.pt-BR.md) | [🇮🇳 हिन्दी](README.hi.md) | [🇯🇵 日本語](README.ja.md) | [🇹🇷 Türkçe](README.tr.md)

## Aperçu
LRP est un protocole de prompting structuré qui sépare contexte, tâche, contraintes et format de sortie, avec une vérification de résonance obligatoire avant exécution.

## Composants clés
1. Couche de contexte
2. Couche de tâche
3. Couche de contraintes
4. Format de sortie

## Vérification de résonance
- Reformuler brièvement le contexte/la tâche/les contraintes interprétés
- Poser une question seulement en cas d’ambiguïté
- Exécuter après alignement

## Démarrage rapide
Vous pouvez utiliser l’outil directement via GitHub Pages : https://irsanai.github.io/LRP-v1.3/

```bash
python3 -m http.server 4173
```
Ouvrir : `http://127.0.0.1:4173/index.html`

## Documentation principale
- [README principal en allemand](README.md)
- [Guide d’utilisation](docs/usage.md)
- [Fonctionnalités](docs/features.md)
- [Feuille de route](docs/professionalization-roadmap.md)
