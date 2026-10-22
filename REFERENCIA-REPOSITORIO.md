# Referência do repositório — Desafio CRM Zero to Hero

**Programa:** Mentoria Zero to Hero IA — Neural Hub  
**Formato:** individual ou dupla  
**Método recomendado:** BMAD  
**Nome sugerido do repositório de referência:** `desafio-crm-zero-to-hero`  
**URL oficial:** https://github.com/Andre-cardia/desafio-crm-zero-to-hero<br>
**Versão deste regulamento:** 22/10/2026.

> **Data limite das apresentações definida: 17/12/2026.** O calendário organiza a abertura em **28/10/2026**, a entrega final do repositório em **14/12/2026, às 23h59**, e a banca em **17/12/2026, das 19h às 22h**. Todos os horários são de **Brasília — America/Sao_Paulo**. Os demais marcos e horários foram planejados para esta turma; a coordenação divulga a programação individual até 10/12. A recuperação posterior não estende o prazo de apresentação.

## 1. Finalidade

Este é o guia central de organização, entrega e avaliação do desafio. O aluno planejará e construirá um CRM interno pequeno: contatos, oportunidades e atividades, com login, dois perfis e uma diferença de permissão verificável no servidor ou na camada de dados.

O trabalho tem dois marcos:

1. **Pré-projeto:** explicar problema, usuários, fluxo, MVP, protótipo e riscos; obter aprovação antes de construir.
2. **Projeto:** revisar o planejamento BMAD, obter aprovação do plano, implementar histórias pequenas, testar e apresentar.

O enunciado e o escopo estão em [DESAFIO.md](DESAFIO.md). A execução está no [tutorial passo a passo](docs/ROTEIRO-PASSO-A-PASSO.md). Este arquivo é a referência de prazos e regras; mudanças devem ser registradas nele e no Issue do marco afetado, com comunicação à turma antes de valerem.

## 2. Como organizar os repositórios

### Repositório da coordenação

Contém o enunciado, regulamento, roteiro, rubrica, modelos e apresentação. A coordenação publica o material no GitHub e pode habilitá-lo como **Template repository**. O instrutor distribui sua URL real à turma.

### Repositório de cada aluno ou dupla

- Criar uma cópia pelo botão **Use this template → Create a new repository**, usando apenas a branch principal do modelo.
- Usar nome identificável, por exemplo `crm-ana-silva` ou `crm-equipe-01`.
- Manter privado durante a avaliação e conceder acesso aos mentores indicados.
- Fazer os Issues e PRs do projeto **na própria cópia**; não enviar o código da atividade ao repositório de referência da coordenação.
- Usar `main` como branch principal; o código e os documentos avaliados devem estar na mesma cópia.
- Preencher no README nome dos participantes, contexto do CRM e links das entregas.

Se o modelo não estiver disponível, a coordenação deve indicar como copiar os arquivos para um repositório vazio. A opção depende de o repositório oficial já ter sido publicado.

## 3. Mapa dos arquivos

| Arquivo ou pasta | Uso |
|---|---|
| [README.md](README.md) | Entrada do repositório e instruções de execução do aplicativo do aluno. |
| [DESAFIO.md](DESAFIO.md) | Problema, MVP obrigatório e definição de pronto. |
| [REFERENCIA-REPOSITORIO.md](REFERENCIA-REPOSITORIO.md) | Prazos, entregas e regras de alunos e mentores. |
| [docs/ROTEIRO-PASSO-A-PASSO.md](docs/ROTEIRO-PASSO-A-PASSO.md) | Preparação, pré-projeto e passos de construção com BMAD. |
| [docs/BOAS-PRATICAS-GITHUB.md](docs/BOAS-PRATICAS-GITHUB.md) | Issues, branches, commits, PRs, documentação e segredos. |
| [docs/AVALIACAO.md](docs/AVALIACAO.md) | Rubrica de 30 + 70 pontos e evidências esperadas. |
| [templates/pre-projeto.md](templates/pre-projeto.md) | Copiar e preencher como `pre-projeto.md` na raiz. |
| [templates/entrega-projeto.md](templates/entrega-projeto.md) | Copiar e preencher como `entrega-projeto.md` na raiz. |
| [templates/ficha-avaliacao.md](templates/ficha-avaliacao.md) | Registro de nota, evidência e feedback de cada mentor. |
| [.github/PULL_REQUEST_TEMPLATE.md](.github/PULL_REQUEST_TEMPLATE.md) | Modelo para descrever mudanças e testes de um PR. |
| [apresentacao.html](apresentacao.html) | Apresentação interativa do desafio. |

**Arquivos que surgem durante o trabalho:** aplicação e testes na estrutura definida pelo plano; `pre-projeto.md`; `entrega-projeto.md`; `.env.example` sem valores secretos; artefatos na pasta de saída configurada pelo BMAD. O repositório de referência não entrega o CRM implementado.

## 4. Responsabilidades

| Papel | Responsabilidade |
|---|---|
| Coordenação | Confirmar calendário, publicar o modelo, distribuir mentores, organizar a banca e decidir exceções documentadas. |
| Aluno ou dupla | Manter repositório acessível, cumprir entregas, revisar IA, demonstrar o produto e responder às perguntas. |
| Mentor relator | Verificar entrega e execução, registrar parecer dos gates e consolidar o feedback no GitHub. |
| Mentor revisor | Avaliar a mesma versão de forma independente e conferir pontuação e falhas críticas. |

Cada projeto terá **dois mentores avaliadores**. Quem tiver conflito de interesse ou tiver implementado parte substancial da entrega deve declarar essa situação à coordenação para redistribuição da avaliação.

## 5. Calendário e data limite

Todas as datas abaixo são de **2026**. Entregas são consideradas pelo horário em que o commit e os links ficam disponíveis aos mentores no GitHub, não pela data de um commit ainda apenas local.

| Data e limite — Brasília | Responsável | Entrega ou decisão |
|---|---|---|
| **28/10, 23h59** | Aluno/dupla | Abrir a cópia individual, identificar participantes e conceder acesso aos mentores. |
| **03/11, 23h59** | Aluno/dupla | Enviar `pre-projeto.md` e protótipo em PR vinculado ao Issue **Marco 1 — Pré-projeto**. |
| **04/11, 19h–22h** | Aluno/dupla | Apresentar o pré-projeto: até 5 minutos + 3 minutos de perguntas. |
| **06/11, 23h59** | Mentores | Publicar **Aprovado** ou **Ajustes necessários** para o Marco 1. |
| **09/11, 23h59 / 10/11, 23h59** | Aluno / mentores | Entregar ajustes do Marco 1 / concluir sua reavaliação. |
| **11/11, 23h59** | Aluno/dupla | Enviar brief, PRD, decisões técnicas e backlog; abrir Issue/PR **Marco 2 — Plano BMAD**. |
| **13/11, 23h59** | Mentores | Aprovar o plano ou listar ajustes objetivos. Só iniciar implementação com os dois gates aprovados. |
| **16/11, 23h59 / 17/11, 23h59** | Aluno / mentores | Entregar ajustes do plano / concluir sua reavaliação. |
| **25/11, 23h59** | Aluno/dupla | Checkpoint 1: acesso, perfis e contatos; registrar funcionamento, pendências e PRs. |
| **02/12, 23h59** | Aluno/dupla | Checkpoint 2: fluxo completo, atividades, testes e permissões; registrar pendências finais. |
| **10/12, 23h59** | Aluno/dupla | Ensaio técnico: testar instalação pelo README, fluxo de demonstração, compartilhamento de tela e vídeo de apoio opcional; registrar checklist no Issue. |
| **10/12, 23h59** | Coordenação | Divulgar ordem, horário individual, sala/link e mentores da apresentação final. |
| **14/12, 23h59** | Aluno/dupla | Entrega final: código, README, artefatos, testes, dados fictícios e `entrega-projeto.md`; publicar tag e hash do commit. |
| **15–16/12, até 23h59 de 16/12** | Mentores | Conferir acesso, executar a versão congelada e preparar perguntas com base na rubrica. |
| **17/12, 19h–22h** | Aluno/dupla e banca | Apresentações finais: até 10 minutos + 5 minutos de perguntas. **Limite para concluir apresentações: 17/12, 22h.** |
| **21/12, 23h59** | Mentores | Publicar nota, parecer, evidências e correções necessárias. |
| **23/12, 23h59** | Aluno/dupla | Prazo para solicitar revisão fundamentada da avaliação. |
| **28/12, 23h59** | Aluno/dupla | Prazo único para enviar correções de recuperação e evidências no PR correspondente. |
| **30/12, 23h59** | Mentores | Encerrar revisão de nota e reavaliação das correções. |

**Capacidade da banca:** reservar 17 minutos por projeto na apresentação final: 10 de apresentação, 5 de perguntas e 2 de transição. Uma sessão de 19h a 22h comporta até 10 projetos, com 10 minutos restantes para intervalo/organização. Havendo mais projetos, a coordenação organiza bancas paralelas ou sessão adicional em 16/12, após a entrega final, e publica a distribuição até 10/12. Nenhuma apresentação regular ultrapassa 17/12, às 22h.

O período de trabalho vai de 28/10 a 17/12, aproximadamente sete semanas. A avaliação e a recuperação encerram em 30/12. Não há nova apresentação regular após 17/12; a recuperação trata somente as pendências registradas.

Os checkpoints são acompanhamento, sem pontuação extra. Caso o mentor atrase um gate, deve registrar a ocorrência e combinar com a coordenação a reorganização do trabalho, sem penalizar o aluno por esse atraso.

## 6. Rotina obrigatória no GitHub

1. **Issue:** o que será feito, por que importa, critérios de aceite e dependências.
2. **Branch curta:** uma história por vez, por exemplo `feat/cadastro-contatos`.
3. **Commits claros:** salvar alterações lógicas, por exemplo `feat: permite cadastrar contatos`.
4. **Verificação:** ler o diff, executar o projeto e testar os critérios.
5. **Pull Request:** informar Issue, mudanças, como testar, resultados, evidências e limitações.
6. **Revisão:** responder comentários e incorporar correções antes do merge.

Exemplo de ciclo, depois de confirmar que a `main` local está limpa:

~~~bash
git switch main
git pull
git switch -c feat/cadastro-contatos

# Depois de implementar, revisar e testar:
git status
git diff
git add CAMINHO_DO_ARQUIVO
git commit -m "feat: permite cadastrar contatos"
git push -u origin feat/cadastro-contatos
~~~

Substitua `CAMINHO_DO_ARQUIVO` pelo arquivo revisado. Na descrição do PR dirigido à branch principal, `Closes #12` associa a mudança ao Issue 12 e permite seu fechamento ao integrar. O número é um exemplo.

**Regras essenciais:** não trabalhar diretamente na `main`; não reescrever o histórico para ocultar decisões; não enviar `.env`, tokens, senhas ou dados reais; usar `.env.example` com nomes das variáveis; manter o README executável. A coordenação configura a exigência de PR/revisão quando o recurso estiver disponível.

## 7. O que entregar em cada marco

### Marco 1 — Pré-projeto

- `pre-projeto.md` completo: problema, usuário, fluxo, escopo, sinais de sucesso e riscos.
- Protótipo de login, contatos, oportunidade e atividade; papel, Figma ou HTML são aceitos.
- Issue e PR com links acessíveis aos mentores.
- Apresentação em 04/11; atender à revisão antes de construir.

### Planejamento do Marco 2

- Brief, PRD, decisões de arquitetura/UX necessárias e histórias com critérios de aceite.
- Artefatos revisados pelo aluno e mantidos dentro do repositório.
- Issue/PR do plano BMAD; aguardar aprovação antes da implementação.

### Entrega final do Marco 2

- Aplicação demonstrável com persistência e fluxo contato → oportunidade → atividade.
- Login/logout, rotas privadas, dois perfis e uma ação negada ao perfil restrito.
- README com instalação, ambiente, banco, execução, testes e limitações.
- Dados fictícios; testes ou checklist reproduzível de fluxo e permissões.
- `entrega-projeto.md` com links dos marcos, PRs, artefatos e evidências.
- Nota sobre uso de IA, decisões humanas e contribuição de cada participante.
- Issue **Entrega final — CRM** com tag **`entrega-final`** e hash completo do commit avaliado.

Após integrar as mudanças aprovadas e conferir o commit correto:

~~~bash
git switch main
git pull
git status
git rev-parse HEAD
git tag -a entrega-final -m "Entrega final do desafio CRM"
git push origin entrega-final
~~~

A tag deve ser criada **uma vez** e permanecer apontando para o commit entregue. Não a mover nem substituí-la. Correções posteriores vão para outro PR e outro commit, ligados à entrega original.

## 8. Regras de apresentação dos alunos

### Pré-projeto — até 5 minutos + 3 de perguntas

| Tempo | Conteúdo |
|---|---|
| 0–1 min | Contexto, problema e impacto. |
| 1–2 min | Usuários e diferença entre os dois perfis. |
| 2–3 min | Fluxo principal e protótipo. |
| 3–4 min | MVP obrigatório e itens fora do escopo. |
| 4–5 min | Viabilidade, principal risco e dúvida que precisa de apoio. |

### Projeto final — até 10 minutos + 5 de perguntas

| Tempo | Conteúdo |
|---|---|
| 0–1 min | Problema e usuário atendido. |
| 1–2 min | Escopo entregue e uma decisão técnica. |
| 2–6 min | Demonstração ao vivo: criar contato, oportunidade, mudar etapa, registrar e concluir atividade. |
| 6–8 min | Perfis, tentativa de operação proibida e evidências de testes. |
| 8–9 min | Repositório, artefatos BMAD e evolução por Issues/PRs. |
| 9–10 min | Uso de IA, limitação conhecida e breve retrospectiva. |

### Condições comuns

- Estar pronto 10 minutos antes do horário individual, com aplicativo iniciado e links testados.
- Em dupla, **os dois apresentam e respondem**; o README informa a contribuição de cada um.
- O aluno compartilha a tela, mostra o produto e explica decisões. Slides são apoio; sua quantidade não é critério de nota.
- Demonstrar o commit congelado da entrega, com dados fictícios. Deploy público é opcional; execução local é aceita.
- Não instalar dependências nem escrever funcionalidades durante a apresentação.
- O mentor avisa quando falta 1 minuto e encerra ao atingir o limite; perguntas vêm depois e não ampliam o tempo de exposição.
- Se houver falha local, usar no máximo 2 minutos **dentro do tempo de apresentação** para recuperar. Uma gravação de apoio de até 3 minutos, da mesma versão entregue, pode mostrar o fluxo; não substitui a checagem técnica do repositório pelos mentores.
- Na arguição, cada integrante deve explicar uma decisão ou mudança de que participou. Se isso não ficar demonstrado, haverá verificação individual na recuperação.

## 9. Regras de avaliação dos mentores

### Pontuação: 100 pontos

| Marco 1 | Máximo |
|---|---:|
| Problema e usuário | 8 |
| Fluxo e escopo | 8 |
| Protótipo | 6 |
| Viabilidade e riscos | 4 |
| Comunicação | 4 |
| **Total do pré-projeto** | **30** |

| Marco 2 | Máximo |
|---|---:|
| Uso do BMAD | 10 |
| Funcionamento do MVP | 25 |
| Acesso e segurança básica | 10 |
| Testes e confiabilidade | 10 |
| GitHub e documentação | 8 |
| Apresentação e reflexão | 7 |
| **Total do projeto** | **70** |

As evidências de cada critério estão em [docs/AVALIACAO.md](docs/AVALIACAO.md).

### Procedimento da banca

1. Conferir acesso ao repositório, links, commit/tag e entregas antes da banca.
2. Avaliar **a mesma versão** e a mesma rubrica; executar o README em ambiente limpo e verificar o fluxo e a permissão proibida. A execução é coordenada pelo relator, com registro para ambos.
3. Cada mentor preenche sua [ficha](templates/ficha-avaliacao.md) de forma independente, com **pontos + evidência + justificativa + ação de melhoria**.
4. Para cada critério, escolher 0%, 25%, 50%, 75% ou 100% do máximo: ausente; incipiente; parcial; atende com lacuna pequena; completo e verificável.
5. Calcular a média dos dois avaliadores por critério. Somar as médias e arredondar a nota total para uma casa decimal, apenas ao final.
6. Diferença superior a 10 pontos no total, ou divergência sobre gate/falha crítica, vai à coordenação para moderação por outro mentor. Registrar quais evidências fundamentaram os ajustes e recalcular a média; não tirar a média de pareceres críticos contraditórios.
7. Publicar parecer único no Issue da entrega, com as fichas e os PRs/commits que sustentam a decisão. Respeitar os prazos do calendário.

**A banca deve:** avaliar o MVP aprovado; aceitar as tecnologias justificadas no plano; reconhecer revisão humana da IA; explicar descontos; registrar limitações não verificadas. Uma execução não testada deve constar como não verificada.

**A banca não deve:** criar requisitos no dia; dar bônus por integração não solicitada; comparar acabamento visual fora da rubrica; premiar ferramenta paga; descontar pontos duas vezes pela mesma falha sem explicar impactos distintos.

### Aprovação

O projeto é aprovado quando atende simultaneamente a:

- **Nota final igual ou superior a 75/100.**
- Marco 1 e plano do Marco 2 aprovados.
- Fluxo obrigatório e persistência demonstráveis; teste de permissão negada verificado.
- Repositório executável e sem falhas críticas pendentes.
- Entrega e apresentação realizadas dentro do calendário ou de exceção formalmente registrada.

Em dupla, a nota técnica do projeto é comum. A conclusão individual também exige participação e capacidade de explicar o trabalho. A pendência de um integrante não reprova automaticamente o outro.

**Impedem aprovação, mesmo com nota suficiente:** segredos/dados reais expostos; acesso indevido à área privada; operação restrita autorizada no servidor/dados; aplicação impossível de executar sem evidência reproduzível; ausência de relação entre problema, MVP e demonstração. Registrar **Pendente de correção**, com teste que comprovará a solução. Não zerar automaticamente critérios sem relação com a falha.

## 10. Atrasos, ausência, revisão e recuperação

- **Pedido de prazo:** registrar no Issue do marco, antes do vencimento, motivo, impacto e nova data solicitada. Não há prorrogação automática; só vale a decisão escrita da coordenação. Em impedimento inesperado, comunicar assim que possível. Reagendamentos de apresentação devem respeitar 17/12, às 22h.
- **Entrega atrasada ou ausente:** fica **Pendente** até decisão registrada. Não se aplica multa de pontos informal; a rubrica continua a mesma. Uma exceção não amplia automaticamente o prazo dos demais.
- **Ausência na banca:** reagendar somente com justificativa aceita e dentro do limite de 17/12, às 22h. Sem apresentação, registrar **Não apresentado** no ciclo regular.
- **Falha geral da sessão:** a coordenação documenta a ocorrência e reorganiza os horários dentro do limite de 17/12, sem atribuir a falha ao aluno. Se isso for impossível, registra a pendência e decide o encaminhamento para outro ciclo; não há extensão automática desta turma.
- **Versão congelada:** após 14/12, correções de execução ou segurança precisam de PR e autorização; conservar o hash original e identificar o novo. Não substituir silenciosamente o que foi entregue.
- **Revisão da nota:** até 23/12, indicar critério, evidência já entregue e motivo do pedido no Issue. A revisão de nota não é oportunidade de adicionar funcionalidade.
- **Recuperação:** uma oportunidade até 28/12 para corrigir itens apontados na banca, retestar e registrar evidências em novo PR. Não é novo escopo nem extensão automática da apresentação regular.
- **Reavaliação até 30/12:** reaplicar os critérios afetados, preservar os demais pontos e publicar o cálculo revisado. Não há teto punitivo de nota; as condições de aprovação continuam iguais.
- Falta de entrega ou apresentação sem exceção aceita exige decisão da coordenação sobre participação em outro ciclo.

## 11. Checklist de uso deste guia

**Coordenação**

- [ ] Divulgar os marcos e destacar a data limite de apresentação: 17/12/2026.
- [x] Publicar o repositório de referência e inserir sua URL real neste documento.
- [ ] Confirmar mentores, capacidade e horários das bancas.
- [ ] Verificar que todos têm acesso às entregas.

**Aluno ou dupla**

- [ ] Criar cópia e compartilhar acesso.
- [ ] Entregar pré-projeto, protótipo e plano BMAD.
- [ ] Aguardar os dois gates antes de implementar.
- [ ] Trabalhar com Issues, branches, commits e PRs.
- [ ] Entregar commit/tag final e apresentar até o limite.

**Mentores**

- [ ] Avaliar a versão entregue com a rubrica comum.
- [ ] Testar execução e permissão proibida.
- [ ] Registrar fichas, evidências, nota e parecer.
- [ ] Responder dentro dos prazos e documentar revisão/recuperação.

## 12. Referências oficiais de uso das ferramentas

- [Criar repositório a partir de modelo — GitHub](https://docs.github.com/pt/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template)
- [GitHub flow](https://docs.github.com/en/get-started/using-github/github-flow)
- [Vincular PR e Issue — GitHub](https://docs.github.com/en/issues/tracking-your-work-with-issues/using-issues/linking-a-pull-request-to-an-issue)
- [Instalação do BMAD](https://docs.bmad-method.org/start/install-bmad/)

A data limite de apresentação, 17/12/2026, foi definida pela coordenação solicitante. Os demais marcos, horários, pesos e regras organizam este desafio; não são exigências do GitHub nem do BMAD.
