# claude-code-plugins

Lista dos plugins do Claude Code que tenho ativos, com a fonte de cada um. **Não copio o código de terceiros**: cada plugin é instalado do repositório original (marketplace), e aqui fica a referência exata.

## Plugins instalados

| Plugin | Marketplace | Repositório | Versão | Descrição |
|---|---|---|---|---|
| `eli5` | `claude-community` | [anthropics/claude-plugins-community](https://github.com/anthropics/claude-plugins-community) | 1.0.0 | Explain any topic like I'm 5: a dead-simple HTML picture explainer with big visuals and few words. Use /eli5 <topic>. |
| `watch` | `claude-video` | [bradautomates/claude-video](https://github.com/bradautomates/claude-video) | 0.3.2 | Give an agent video evidence: timestamped frames and native captions, with optional local WhisperX or Groq/OpenAI transcription. |
| `impeccable` | `impeccable` | [pbakaus/impeccable](https://github.com/pbakaus/impeccable) | 4.5.2 | Design fluency for frontend development. 1 skill with 24 commands (/impeccable polish, /impeccable audit, /impeccable critique, etc.) and curated anti-pattern detection. |
| `ponytail` | `ponytail` | [DietrichGebert/ponytail](https://github.com/DietrichGebert/ponytail) | 5.1.0 | Lazy senior dev mode. Forces the simplest, shortest solution that actually works: YAGNI, stdlib first, no unrequested abstractions. |
| `skins` | `hellosverre-mods` | [hellosverre/claude-skins](https://github.com/hellosverre/claude-skins) | 0.5.3 | Skins for Claude Code: tool rows that open onto their input and answer, highlighted code, diff, table, math, Mermaid and shell cards, links, folding, a usage band, a calm mode and fifteen themes. /skin swaps them live. |
| `mods-manager` | `mods-manager` | [ptpmediabr/mods-manager](https://github.com/ptpmediabr/mods-manager) | 0.4.4 | Painel para ver, ligar, desligar, instalar e agrupar em perfis os seus mods e plugins. |
| `usage-weather` | `usage-weather` | [ptpmediabr/usage-weather](https://github.com/ptpmediabr/usage-weather) | 0.2.2 | One quiet line above the prompt: context, 5-hour and weekly usage, whether the prompt cache is warm, and a Clear & continue button. |
| `ideas-shelf` | `ideas-shelf` | [ptpmediabr/ideas-shelf](https://github.com/ptpmediabr/ideas-shelf) | 0.1.0 | Prateleira de ideias por projeto: anote ideias num painel e marque como feitas; fica salvo em IDEAS.md na raiz do projeto. |
| `side-chat` | `side-chat` | [ptpmediabr/side-chat](https://github.com/ptpmediabr/side-chat) | 0.2.0 | A side chat pane inside the session that answers questions or runs requests on a model of your choice. |

Os arquivos:

- [`plugins.json`](plugins.json): versão, commit exato e status de cada plugin.
- [`settings.example.json`](settings.example.json): o bloco de `enabledPlugins` e `extraKnownMarketplaces` para copiar no seu `~/.claude/settings.json`. Não inclui permissões, hooks nem variáveis de ambiente.

## Como instalar (no terminal, com `claude`)

Adicione os marketplaces e instale cada plugin:

```text
/plugin marketplace add <owner/repo>
/plugin install <plugin>@<marketplace>
```

Os repositórios estão na tabela acima. Os comandos `/plugin` rodam no terminal interativo do `claude`.

## Marketplaces registrados sem plugin instalado

- `claude-plugins-official` (anthropics/claude-plugins-official)
