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

## Material de referência
- `Resumo_DE_Jackson5.md`: contexto completo do desafio e das decisões.
- Documento "Jackson 5 — Escopo e Plano do Projeto" (Claude Docs): https://claude.ai/artifact/EjaqgdsXqZq4CY9mpp1Qek
- Slides do Conecta: https://claude.ai/artifact/8ydd3b1oFadGRwpXDH46wq
- `entregas/Orcamento_PoC_Jackson5.xlsx`: orçamento da PoC e esqueleto do MVP.
- Edital completo do 4º Prêmio Inova+Saúde: https://www.bahiana.edu.br/premio-inova-saude/ (prazo 10/12/2026, 18h).

## Agentes da equipe (`.claude/agents/`)
| Agente | Quando usar |
|---|---|
| `especialista-edital` | Proposta do Prêmio Inova+Saúde: elegibilidade, documentos, texto alinhado aos critérios e pesos, plano da PoC e do MVP. |
| `especialista-saas` | Arquitetura, stack, real x simulado, treino e avaliação da IA, integrações, segurança técnica, custos de nuvem. |
| `pesquisa-clinica` | Formulário de sintomas, regra de prioridade, estudo de validação da PoC, protocolo e TCLE para o CEP, viés por tom de pele. |
| `analista-mercado` | AV2: concorrentes, diferenciação, proposta de valor, TAM/SAM/SOM, roteiros e análise de entrevistas. |
| `regulacao-lgpd` | Revisar textos, telas e planos sob ANVISA, CFM, LGPD e ética em pesquisa; estratégia regulatória. |
| `financas-av3` | Orçamento do edital, preço, custos, break-even, unit economics, AV3. |
| `coach-pitch` | Roteiros (Conecta, vídeo do edital, D.E) e simulação de banca. |
| `revisor-avaliacoes` | Completar e revisar AV1, AV2 e AV3 contra o formulário oficial e checar coerência entre entregas. |

Exemplo: "use o analista-mercado para montar a tabela de concorrentes da AV2".
