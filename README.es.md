# IrsanAI · LRP v1.3

> 🌍 **Lee este README en tu idioma:**
> [🇬🇧 English](README.en.md) | [🇩🇪 Deutsch](README.md) | [🇪🇸 Español](README.es.md) | [🇮🇹 Italiano](README.it.md) | [🇧🇦 Bosanski](README.bs.md) | [🇷🇺 Русский](README.ru.md) | [🇨🇳 中文](README.zh.md) | [🇫🇷 Français](README.fr.md) | [🇧🇷 Português (BR)](README.pt-BR.md) | [🇮🇳 हिन्दी](README.hi.md) | [🇯🇵 日本語](README.ja.md) | [🇹🇷 Türkçe](README.tr.md)

## Resumen
LRP es un protocolo de prompting estructurado que separa contexto, tarea, restricciones y formato de salida, con verificación de resonancia obligatoria antes de ejecutar.

## Componentes clave
1. Capa de contexto
2. Capa de tarea
3. Capa de restricciones
4. Formato de salida

## Verificación de resonancia
- Repite brevemente contexto/tarea/restricciones interpretados
- Pregunta solo si hay ambigüedad
- Ejecuta después de la alineación

## Inicio rápido
Puedes usar la herramienta directamente en GitHub Pages: https://irsanai.github.io/LRP-v1.3/

```bash
python3 -m http.server 4173
```
Abrir: `http://127.0.0.1:4173/index.html`

## Documentación principal
- [README principal en alemán](README.md)
- [Guía de uso](docs/usage.md)
- [Funciones](docs/features.md)
- [Hoja de ruta](docs/professionalization-roadmap.md)
