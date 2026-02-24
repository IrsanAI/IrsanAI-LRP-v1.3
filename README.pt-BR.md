# IrsanAI · LRP v1.3

> 🌍 **Leia este README no seu idioma:**
> [🇬🇧 English](README.en.md) | [🇩🇪 Deutsch](README.md) | [🇪🇸 Español](README.es.md) | [🇮🇹 Italiano](README.it.md) | [🇧🇦 Bosanski](README.bs.md) | [🇷🇺 Русский](README.ru.md) | [🇨🇳 中文](README.zh.md) | [🇫🇷 Français](README.fr.md) | [🇧🇷 Português (BR)](README.pt-BR.md) | [🇮🇳 हिन्दी](README.hi.md) | [🇯🇵 日本語](README.ja.md) | [🇹🇷 Türkçe](README.tr.md)

## Visão geral
LRP é um protocolo de prompting estruturado que separa contexto, tarefa, restrições e formato de saída, com checagem de ressonância obrigatória antes da execução.

## Componentes principais
1. Camada de contexto
2. Camada de tarefa
3. Camada de restrições
4. Formato de saída

## Checagem de ressonância
- Repetir brevemente contexto/tarefa/restrições interpretados
- Perguntar apenas se houver ambiguidade
- Executar após alinhamento

## Início rápido
Você pode usar a ferramenta diretamente pelo GitHub Pages: https://irsanai.github.io/LRP-v1.3/

```bash
python3 -m http.server 4173
```
Abrir: `http://127.0.0.1:4173/index.html`

## Documentação principal
- [README principal em alemão](README.md)
- [Guia de uso](docs/usage.md)
- [Funcionalidades](docs/features.md)
- [Roteiro](docs/professionalization-roadmap.md)
