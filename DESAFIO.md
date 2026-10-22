# Desafio aplicado — CRM interno simplificado

**Mentoria:** Zero to Hero IA  
**Formato:** individual ou dupla  
**Duração:** aproximadamente 7 semanas, de 28/10 a 17/12/2026<br>
**Metodologia recomendada:** BMAD Method  
**Entrega:** aplicação demonstrável e repositório GitHub com histórico de trabalho

## 1. O desafio

Planeje e construa um CRM interno para ajudar uma pessoa ou pequena equipe a acompanhar contatos, oportunidades comerciais e próximos passos. O projeto deve resolver um problema real e ter escopo pequeno o bastante para ser concluído durante a mentoria.

Não é necessário criar um CRM para venda como SaaS. Não implemente cobrança, múltiplas empresas isoladas, marketplace ou integrações complexas.

## 2. Fluxo principal

O CRM deve permitir que a equipe:

1. registre um contato;
2. crie uma oportunidade associada ao contato;
3. acompanhe a oportunidade em etapas simples, como **Novo → Em conversa → Proposta → Ganho/Perdido**;
4. registre uma atividade ou próximo passo com data;
5. consulte e atualize os registros conforme seu perfil de acesso.

## 3. MVP obrigatório

- **Acesso:** login e logout; rotas privadas; dois perfis simples, por exemplo administrador e operador.
- **Contatos:** criar, visualizar, editar, pesquisar e arquivar ou excluir conforme a regra definida.
- **Oportunidades:** criar, editar, atribuir uma etapa e marcar como ganha ou perdida.
- **Atividades:** registrar uma tarefa ou reunião, definir prazo e marcar como concluída.
- **Permissões:** pelo menos uma diferença verificável entre os perfis. A verificação precisa acontecer no servidor ou na camada de dados, além da interface.
- **Qualidade:** validação de campos, estados de carregamento/erro, dados fictícios e instruções para executar o projeto.

Um painel simples com totais de oportunidades e atividades pode ser incluído se o fluxo obrigatório já estiver funcionando.

## 4. Fora do escopo obrigatório

- Cadastro público aberto ou cobrança.
- Aplicativo móvel nativo.
- Integração com e-mail, calendário ou WhatsApp.
- IA conversacional dentro do CRM.
- Importação/exportação em lote, anexos ou campos personalizados.
- Arquitetura distribuída, microserviços ou múltiplos tenants.

Esses itens só entram se forem necessários ao problema escolhido e aprovados pelo instrutor.

## 5. Dois marcos de avaliação

### Marco 1 — Pré-projeto: decidir o que vale construir

O aluno explica o problema e demonstra que o MVP é viável antes de começar a implementação.

**Entregáveis:**

- `pre-projeto.md`, preenchido a partir do [modelo](templates/pre-projeto.md);
- protótipo simples das telas centrais, que pode ser feito em papel, Figma ou HTML;
- apresentação de até 5 minutos.

O marco é aprovado quando o instrutor consegue entender quem usa o CRM, qual problema ele resolve, qual é o fluxo principal e o que ficou fora do MVP. Após a aprovação, o escopo pode ser ajustado pelo GitHub Issue.

### Marco 2 — Projeto: planejar, construir e demonstrar

O aluno usa os artefatos BMAD para guiar a construção do fluxo principal, acompanha o trabalho no GitHub e apresenta uma versão funcional.

**Entregáveis mínimos no repositório:**

- artefatos de produto e planejamento gerados com BMAD;
- aplicação com o fluxo principal funcionando;
- instruções de instalação e execução no `README.md` do projeto;
- testes ou checklist documentado dos fluxos principais e das permissões;
- dados fictícios para demonstração;
- apresentação de até 10 minutos e breve retrospectiva.

Não é preciso produzir um conjunto extenso de documentos separados. O PRD, a arquitetura, as histórias e o plano de implementação podem permanecer nos arquivos que o BMAD gerar. O aluno deve manter apenas os artefatos necessários para explicar e executar o projeto.

## 6. Regras de uso de IA

- O aluno responde pelas decisões, pelo código enviado e pela demonstração.
- Revise cada mudança sugerida pela IA; não aceite código sem entender seu efeito.
- Não permita que a IA invente requisitos, dados ou credenciais.
- Registre no README uma breve nota sobre onde a IA ajudou e onde foi necessário corrigir ou rejeitar uma sugestão.
- Não cole segredos, dados reais de clientes ou arquivos confidenciais em ferramentas de IA.

## 7. Definição de pronto

O projeto está pronto para avaliação quando:

- o fluxo contato → oportunidade → atividade pode ser demonstrado;
- os dois perfis têm permissões diferentes e a regra foi testada;
- o projeto inicia seguindo as instruções do README;
- os testes/checklists e limitações conhecidas estão documentados;
- o repositório não contém segredos nem dados pessoais reais;
- o histórico do GitHub mostra trabalho incremental, não apenas um envio final.

## 8. Prazos, apresentações e avaliação

**Data limite de apresentação: 17/12/2026.** Todos os horários são de Brasília (America/Sao_Paulo). Os demais marcos e horários organizam o trabalho até essa data; a programação individual da banca será divulgada até 10/12.

| Marco | Prazo |
|---|---|
| Abertura e acesso ao repositório | 28/10/2026, até 23h59 |
| Entrega do pré-projeto e protótipo | 03/11/2026, até 23h59 |
| Apresentação do pré-projeto | 04/11/2026, das 19h às 22h |
| Parecer dos mentores sobre o pré-projeto | 06/11/2026, até 23h59 |
| Entrega do plano BMAD | 11/11/2026, até 23h59 |
| Parecer dos mentores sobre o plano | 13/11/2026, até 23h59 |
| Checkpoints de desenvolvimento | 25/11 e 02/12/2026, até 23h59 |
| Ensaio técnico e divulgação dos horários da banca | 10/12/2026, até 23h59 |
| Entrega final do repositório | **14/12/2026, até 23h59** |
| Apresentações finais | **17/12/2026, das 19h às 22h; limite de conclusão: 22h** |
| Nota e feedback da banca | 21/12/2026, até 23h59 |
| Pedido de revisão / correções de recuperação | 23/12 / 28/12/2026, até 23h59 |
| Encerramento da reavaliação | 30/12/2026, até 23h59 |

- Pré-projeto: até **5 minutos + 3 de perguntas**. Projeto final: até **10 minutos + 5 de perguntas**.
- Em dupla, ambos apresentam e respondem. Demonstrar a versão entregue, usando dados fictícios; execução local é aceita.
- Entregar a tag `entrega-final` e o hash do commit. Manter a versão original; correções posteriores exigem outro PR.
- Dois mentores avaliam pela mesma rubrica: **30 pontos no pré-projeto + 70 no projeto**.
- Aprovação: **pelo menos 75/100**, gates aprovados, fluxo e permissões verificados e nenhuma falha crítica pendente.
- A recuperação até 28/12 trata correções e não prorroga as apresentações, que devem terminar em 17/12.

As regras completas, os horários de banca, os prazos de ajustes dos gates e os procedimentos de atraso, avaliação e revisão estão em [REFERENCIA-REPOSITORIO.md](REFERENCIA-REPOSITORIO.md).
