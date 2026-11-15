# Jackson 5 — Desafio Empreendedor 2026.2

Pasta de trabalho da equipe Jackson 5 (Universidade SENAI CIMATEC, Salvador) no Desafio Empreendedor 2026.2, pilar 1 (apoio ao diagnóstico, tratamento e/ou prevenção).

**Fonte principal de contexto:** `Resumo_DE_Jackson5.md`. Leia antes de qualquer tarefa. Ele traz as regras do desafio, as decisões da equipe, o estado da AV1, os pontos de atenção e os próximos passos.

## A ideia em uma frase
App gratuito para o paciente fotografar uma lesão de pele e responder a um formulário de sintomas. A IA gera uma triagem com nível de prioridade, que vai para uma clínica assinante (SaaS B2B, na prática B2B2C). A clínica contata o paciente e agenda a consulta.

## Regras que valem para qualquer trabalho aqui
- **Nunca autodiagnóstico.** O paciente vê só a orientação e o nível de prioridade, nunca a hipótese da IA. A decisão diagnóstica é sempre do médico. Para o paciente, use "triagem" ou "avaliação de prioridade", não "pré-diagnóstico".
- **Não invente dados.** Números de entrevistas, cartas de intenção, preços de concorrentes e estatísticas só entram com fonte real. Se faltar, marque como `[PENDENTE: ...]` e diga o que a equipe precisa levantar.
- **Cite fontes** com link nas afirmações de mercado, saúde e regulação. Prefira fontes primárias (INCA, ANVISA, CFM, artigos).
- **Foco no pitch.** A função secundária (exames e receitas) fica fora da AV1 e da AV2. Pode aparecer na AV3 só como módulo futuro.
- Escreva em português, de forma direta, pensando que o leitor é um estudante de engenharia com pouco tempo.
- Os arquivos em `D. E/Anexos/` são originais: não altere. Gere versões novas com o sufixo `_Jackson5`.

## Agentes da equipe (`.claude/agents/`)
| Agente | Quando usar |
|---|---|
| `especialista-saas` | Arquitetura, stack, protótipo para a banca, IA, integrações, roadmap em 3 fases. |
| `analista-mercado` | AV2: concorrentes, diferenciação, proposta de valor, TAM/SAM/SOM. |
| `regulacao-lgpd` | Revisar qualquer texto ou decisão de produto sob ANVISA (SaMD), CFM e LGPD. |
| `financas-av3` | AV3: preço, custos, break-even, planilha de viabilidade. |
| `coach-pitch` | Roteiro do pitch de 3 a 5 min e simulação de perguntas da banca. |
| `revisor-avaliacoes` | Completar e revisar as AV1, AV2 e AV3 (.docx) contra o formulário oficial. |

Exemplo: "use o analista-mercado para montar a tabela de concorrentes da AV2".
