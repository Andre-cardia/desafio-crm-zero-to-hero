# Avaliação do desafio

Há dois marcos, com feedback no GitHub. O Marco 1 é um gate: o aluno precisa obter aprovação antes de começar a implementação.

O plano BMAD também exige aprovação antes da execução das histórias. Consulte [prazos e regras da banca](../REFERENCIA-REPOSITORIO.md) e use a [ficha de avaliação](../templates/ficha-avaliacao.md).

## Aplicação da rubrica

- Dois mentores avaliam a mesma versão de forma independente e justificam os pontos por evidência.
- Por critério, usar 0%, 25%, 50%, 75% ou 100% do máximo. Calcular a média dos dois mentores por critério e arredondar apenas a soma final para uma casa decimal.
- Diferença de mais de 10 pontos entre os totais ou divergência sobre falha crítica exige moderação pela coordenação antes do parecer.
- **Aprovação final: 75/100 ou mais**, com os dois gates aprovados, fluxo obrigatório e permissões verificados, entrega/apresentação realizadas e ausência de falha crítica.
- Nota suficiente com impedimento crítico resulta em **Pendente de correção**, até reavaliação. Não há bônus por extras fora do MVP.
- No calendário da turma, feedback até **21/12/2026**, pedido de revisão até **23/12**, correções até **28/12** e reavaliação até **30/12**, sempre às 23h59 de Brasília.

**Antes da banca:** a entrega congela em 14/12, às 23h59. Os mentores verificam acesso e execução em 15–16/12 e avaliam as apresentações até 17/12, às 22h. Recuperação e revisão posteriores não reabrem o prazo de apresentação.

## Marco 1 — Pré-projeto (30 pontos)

| Critério | Pontos | O que será observado |
|---|---:|---|
| Problema e usuário | 8 | Contexto concreto, usuário identificável e impacto explicado |
| Fluxo e escopo | 8 | Caminho principal claro; MVP pequeno; itens fora de escopo definidos |
| Protótipo | 6 | Telas suficientes para entender o fluxo sem exigir acabamento visual |
| Viabilidade e riscos | 4 | Plano possível no prazo e riscos principais reconhecidos |
| Comunicação | 4 | Apresentação direta, consistente com o documento |

**Gate de aprovação:** problema, usuário e MVP compreensíveis; protótipo representa o fluxo; escopo cabe no prazo. O instrutor registra **Aprovado** ou **Ajustes necessários** no PR.

## Marco 2 — Projeto (70 pontos)

| Critério | Pontos | O que será observado |
|---|---:|---|
| Uso do BMAD | 10 | Brief/PRD, decisões e tarefas coerentes; aluno revisou os artefatos |
| Funcionamento do MVP | 25 | Contato → oportunidade → atividade é demonstrável e persiste os dados |
| Acesso e segurança básica | 10 | Dois perfis têm diferença real; segredos e dados pessoais não foram expostos |
| Testes e confiabilidade | 10 | Fluxos principais e tentativa de acesso proibido foram verificados |
| GitHub e documentação | 8 | Issues, commits e PRs claros; README permite rodar o projeto |
| Apresentação e reflexão | 7 | Demonstração, limitações e uso da IA explicados com clareza |

## Faixas de desempenho

- **90–100:** MVP consistente, bem validado e processo claro.
- **75–89:** MVP funcional, com pequenas lacunas documentadas.
- **60–74:** fluxo principal parcialmente concluído; falhas ou limites ainda impedem a demonstração completa.
- **Abaixo de 60:** requisitos centrais não foram demonstrados ou o trabalho não pode ser reproduzido.

## Evidências para avaliação

- PR do pré-projeto aprovado;
- Issues e PRs do plano BMAD e das histórias principais;
- aplicação executando;
- dados fictícios;
- evidência dos testes e das permissões;
- README e limitações conhecidas;
- apresentação final.

## Falhas que impedem aprovação final até correção

- segredo, chave de API ou dado real de cliente no repositório;
- usuário sem acesso conseguindo abrir área privada;
- perfil restrito executando no servidor uma operação que deveria ser negada;
- aplicação impossível de iniciar e ausência de evidência reproduzível;
- falta de relação verificável entre o problema, o MVP e a demonstração.
