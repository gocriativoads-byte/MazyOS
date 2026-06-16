# Clínica de Estética — MazyOS

Operação da clínica. O sistema organiza conteúdo, comunicação e processos de uma clínica de estética com referência em otoplastia, rejuvenescimento íntimo, harmonização, estética, odontologia e podologia.

**Estrutura de pastas:**
- `_memoria/` — quem é a clínica, como falamos, foco atual
- `identidade/` — marca aplicada em tudo que o sistema gera
- `marketing/` — campanhas, conteúdo, Instagram, mídia paga
- `saidas/` — documentos e materiais pontuais
- `dados/` — arquivos a analisar
- `scripts/` — automações e scripts de apoio

## Sobre a clínica

Clínica de estética com referência em ajuste de orelhas (otoplastia) e rejuvenescimento íntimo. Também atua em harmonização facial, estética geral, odontologia e podologia. Atende mulheres de alto nível com equipe multidisciplinar.

## O que mais fazemos aqui

- Postagens e conteúdo para Instagram
- Comunicação com clientes (textos, legendas, mensagens)
- Campanhas de marketing digital
- Materiais de divulgação dos procedimentos

## Tom de voz

Direto, convidativo e elegante. Referência real: *"venha nos conhecer e entender a excelência no serviço."*

Evitar: mensagens longas, áudios extensos, linguagem genérica, promessas vazias.

## Regras do sistema

- Conteúdo de Instagram vai em `marketing/`
- Materiais e documentos avulsos vão em `saidas/`
- Antes de criar qualquer visual, consultar `identidade/design-guide.md`
- Identidade visual ainda em construção — preencher o design-guide assim que definir cores, fontes e logo

## Ferramentas conectadas

- [ ] Meta Ads
- [ ] Google Ads
- [ ] Instagram (Meta Graph API)
- [ ] Notion
- [ ] Gmail

*(Marcar conforme for instalando os MCPs)*

---

## Contexto do negócio

No início de toda conversa, ler os seguintes arquivos (quando existirem e estiverem preenchidos):

1. `_memoria/empresa.md` — quem é a clínica, o que faz, como funciona
2. `_memoria/preferencias.md` — tom de voz, estilo de escrita, o que evitar
3. `_memoria/estrategia.md` — foco atual, prioridades, prazos

Usar essas informações como base pra qualquer resposta ou decisão. Não é necessário listar o que foi lido nem confirmar a leitura — apenas usar o contexto naturalmente.

Pra qualquer tarefa visual (carrossel, post, landing page), consultar `identidade/design-guide.md` como referência de estilo.

---

## Fluxo de trabalho

Antes de executar qualquer tarefa, verificar se existe skill relevante em `.claude/skills/`. Se encontrar, seguir as instruções da skill. Se não encontrar, executar a tarefa normalmente.

Ao concluir uma tarefa que não tinha skill mas parece repetível, perguntar:

> "Isso pode virar uma skill pra próxima vez. Quer que eu crie?"

---

## Aprender com correções

Quando o usuário corrigir algo ou dar instrução permanente, perguntar:

> "Quer que eu salve isso pra não precisar repetir?"

Se sim, salvar em:
- **Sobre o negócio** → `_memoria/empresa.md`
- **Sobre preferências e estilo** → `_memoria/preferencias.md`
- **Sobre prioridades** → `_memoria/estrategia.md`
- **Regra de comportamento** → `CLAUDE.md`

---

## Criação de skills

Quando o usuário pedir skill nova, verificar templates em `templates/skills/`, perguntar se é específica desse projeto ou universal, e seguir o fluxo da skill-creator nativa do Claude Code.
