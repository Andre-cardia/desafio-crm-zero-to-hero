# Tutorial passo a passo — do pré-projeto ao CRM

Este roteiro foi pensado para quem está começando. Siga a ordem e use BMAD como apoio para pensar, documentar e implementar. Você continua responsável por aprovar decisões e conferir o resultado.

Antes de começar, leia [REFERENCIA-REPOSITORIO.md](../REFERENCIA-REPOSITORIO.md): calendário da turma, regras de apresentação, entrega por commit/tag e critérios da banca. A entrega final está prevista para **14/12/2026, às 23h59** e o limite definido para as apresentações é **17/12/2026, às 22h**, horário de Brasília.

## Antes de começar

Tenha:

- uma conta GitHub;
- Git instalado e configurado;
- Node.js 20.12 ou superior, Python 3.10 ou superior e `uv` para o BMAD estável;
- Codex ou outra ferramenta de programação compatível com as instruções BMAD;
- um editor de código e acesso ao terminal.

Consulte a [página oficial de instalação do BMAD](https://docs.bmad-method.org/start/install-bmad/). Ela diferencia a versão estável 6.12 da versão 7 em preview. Para este desafio, prefira a estável e não misture os dois métodos de instalação.

## Etapa 0 — Preparar o repositório de avaliação

O instrutor publica este material como repositório de referência. Cada aluno trabalha em uma cópia individual.

1. Abra o repositório de referência fornecido pelo instrutor.
2. Selecione **Use this template → Create a new repository**. Se essa opção não existir, siga a forma de cópia indicada pelo instrutor.
3. Use um nome identificável, por exemplo `crm-andre-silva`.
4. Escolha a visibilidade combinada com o instrutor. Se for privado, convide o instrutor em **Settings → Collaborators**.
5. Clone o repositório para o computador:

   ```bash
   git clone https://github.com/SEU-USUARIO/SEU-REPOSITORIO.git
   cd SEU-REPOSITORIO
   ```

6. Confirme que está na pasta certa e que o repositório está limpo:

   ```bash
   git status
   ```

7. Leia `DESAFIO.md`, este roteiro e a rubrica em `docs/AVALIACAO.md`.

## Marco 1 — Pré-projeto

### Passo 1 — Escolha um contexto realista

Escolha uma atividade comercial simples que você conheça. Pode ser acompanhamento de clientes, vendas de serviços ou organização de contatos de uma pequena equipe. Não use dados reais no projeto.

Responda em `templates/pre-projeto.md`:

- Quem sente o problema?
- Como o trabalho é feito hoje?
- O que se perde ou atrasa?
- Qual melhoria seria perceptível após usar o CRM?

### Passo 2 — Descreva dois perfis de usuário

Comece apenas com **Administrador** e **Operador**. Escreva o que cada um pode fazer e escolha uma ação que o operador não pode executar. Não crie uma matriz extensa de permissões.

### Passo 3 — Desenhe um fluxo principal

Registre de 4 a 6 etapas desde o primeiro contato até o fechamento. Exemplo:

`Novo contato → Primeiro contato → Proposta → Negociação → Ganho ou perdido`

Anote também o próximo passo que costuma ser esquecido e que virará uma atividade no CRM.

### Passo 4 — Defina o MVP

Preencha o que é **obrigatório**, o que pode esperar e o que fica fora. Use o fluxo do `DESAFIO.md` como limite. Cada funcionalidade obrigatória deve resolver parte do problema descrito.

### Passo 5 — Faça um protótipo rápido

Desenhe as telas necessárias para demonstrar o fluxo: login, lista/detalhe de contato, oportunidade por etapa e atividade. Podem ser esboços, wireframes ou um protótipo clicável. Não programe ainda.

### Passo 6 — Peça apoio ao BMAD para revisar o pré-projeto

Depois de instalar e iniciar o BMAD (veja a seção “Preparar BMAD”), peça uma revisão, por exemplo:

> Revise meu pré-projeto para um CRM interno. Identifique contradições, itens grandes demais para o MVP e perguntas que preciso responder. Não invente respostas; pergunte antes de alterar o escopo. Ainda não escreva código.

Leia a revisão, corrija o documento e registre as decisões tomadas. A IA não aprova a etapa; o instrutor faz essa avaliação.

### Passo 7 — Entregue e aguarde o gate

Crie um Issue chamado **Marco 1 — Pré-projeto**, anexe ou referencie o protótipo e abra um Pull Request (PR) com o documento preenchido. Apresente em até 5 minutos. Corrija os comentários do instrutor no próprio PR.

**Não inicie a construção do CRM até receber aprovação do Marco 1.**

## Preparar BMAD para o projeto

Faça esta etapa depois de decidir onde ficará o código. No terminal, dentro da pasta raiz do repositório:

1. Confira os pré-requisitos: `node --version`, `python --version` e `git --version`.
2. Instale o BMAD estável com o comando oficial:

   ```bash
   npx bmad-method install
   ```

3. No assistente de instalação, selecione o método principal e a ferramenta que você usará. Evite instalar várias metodologias/módulos que não fazem parte deste desafio.
4. Abra o projeto na ferramenta de IA escolhida e use a ajuda do BMAD para confirmar a instalação e conhecer os workflows disponíveis. A documentação e os nomes de comandos podem mudar entre versões; use os que sua instalação apresenta.
5. Confirme que os arquivos de configuração e de saída do BMAD ficaram dentro deste repositório. Não instale uma segunda versão do BMAD por outro método no mesmo projeto.

Se o instalador oferecer uma versão em preview, permaneça na versão estável para esta turma. Consulte a documentação oficial se os requisitos ou os passos da instalação tiverem mudado.

## Marco 2 — Projeto

### Passo 8 — Transforme o pré-projeto em um brief

Peça ao workflow de **Product Brief/Project Brief** do BMAD para ler `pre-projeto.md` e produzir um brief curto. Diga explicitamente:

> Use somente as informações do pré-projeto. Liste dúvidas em aberto em vez de completar lacunas por conta própria. Mantenha o escopo limitado ao MVP aprovado. Guarde o artefato dentro da pasta de saída BMAD deste repositório.

Revise o resultado e atualize o arquivo se sua decisão humana divergir.

### Passo 9 — Gere e revise o PRD

Use o workflow **PRD** do BMAD com o brief aprovado. Solicite apenas o necessário:

- objetivo e usuários;
- fluxo principal;
- requisitos do MVP;
- regras do Administrador e Operador;
- critérios de aceite verificáveis;
- limites e questões em aberto.

Confirme que o PRD não incluiu módulos excluídos do desafio. Se tiver incluído, corte ou mova para “fora do MVP”.

### Passo 10 — Planeje a solução e as tarefas

Peça ao BMAD que recomende se o projeto precisa de desenho de UX e arquitetura técnica. Para um CRM novo, produza uma arquitetura simples e justifique as escolhas. Evite adicionar serviços só porque a IA os sugeriu.

Em seguida, peça para dividir o MVP em poucas histórias pequenas, cada uma com critérios de aceite. Um plano possível:

1. estrutura inicial e instruções para rodar;
2. login e perfis;
3. contatos;
4. oportunidades e etapas;
5. atividades e prazos;
6. testes, dados fictícios e revisão.

Histórias menores são mais fáceis de revisar do que um pedido para gerar o CRM inteiro de uma vez.

### Passo 11 — Aprove o plano no GitHub

Abra um Issue **Marco 2 — Plano BMAD** com links para o brief, PRD, decisões técnicas e backlog. Abra um PR com os artefatos. Faça o instrutor aprovar o escopo e o plano antes de executar as histórias.

### Passo 12 — Implemente uma história por vez

Para cada história aprovada:

1. abra ou atualize o Issue correspondente;
2. crie uma branch curta a partir da `main`;
3. peça ao BMAD para implementar somente aquela história e consultar os critérios de aceite;
4. leia o diff, rode o projeto e execute os testes;
5. corrija falhas antes de abrir o PR;
6. abra um PR pequeno e peça revisão;
7. incorpore o feedback e só então integre a branch.

Exemplo de prompt:

> Implemente somente a história #12. Antes, resuma os arquivos que pretende alterar e como os critérios de aceite serão atendidos. Não faça outras histórias. Depois, execute os testes relevantes e relate qualquer critério que não conseguiu verificar.

### Passo 13 — Teste o caminho completo

Com dados fictícios, faça uma demonstração do início ao fim:

1. entrar com cada perfil;
2. criar um contato;
3. criar uma oportunidade para esse contato;
4. mudar a oportunidade de etapa;
5. registrar uma atividade e concluí-la;
6. tentar executar a ação proibida para o Operador;
7. confirmar que a permissão é recusada também no servidor/dados.

Registre o resultado no PR ou no Issue do Marco 2. Se algo falhar, descreva o defeito e corrija antes da entrega final.

### Passo 14 — Feche o projeto

Atualize o README do aplicativo com instalação, configuração, execução, testes, dados de demonstração e limitações. Apresente o produto em até 10 minutos e explique uma decisão de escopo, uma decisão de implementação, o que a IA ajudou a fazer e o que você revisou ou rejeitou.

## Modelo curto de prompts BMAD

Use os workflows instalados pelo BMAD e adapte a linguagem do pedido:

1. **Brief:** “Crie um brief a partir do pré-projeto. Não invente dados; liste dúvidas.”
2. **PRD:** “Crie o PRD do MVP aprovado, com requisitos e critérios testáveis.”
3. **Arquitetura:** “Proponha a arquitetura mínima para estes requisitos. Compare escolhas e explique custos e limites.”
4. **Backlog:** “Divida o MVP em histórias pequenas, em ordem de dependência, sem adicionar escopo.”
5. **Implementação:** “Implemente apenas a história X. Mostre plano, diff, testes e itens não verificados.”
6. **Revisão:** “Revise o PR e procure bugs, permissões incorretas, dados expostos e critérios de aceite ausentes. Não aplique correções sem explicar o achado.”

## Se algo der errado

- **BMAD gerou documento longo demais:** peça um resumo e mantenha o arquivo detalhado gerado, mas use somente as decisões necessárias no trabalho.
- **A IA ampliou o escopo:** volte ao MVP aprovado e abra um Issue para qualquer nova ideia.
- **O teste falhou:** copie a mensagem de erro sem chaves ou dados pessoais, reproduza o problema e peça ajuda para diagnosticar antes de alterar várias partes.
- **A aplicação não está pronta para deploy:** demonstre localmente e registre essa limitação; não apresente uma URL quebrada como entrega concluída.
- **Perdeu o trabalho local:** recupere pela branch remota com `git pull` ou clone novamente o repositório.

## Fontes oficiais

- [Instalação do BMAD](https://docs.bmad-method.org/start/install-bmad/)
- [Escolher um caminho de planejamento](https://docs.bmad-method.org/plan/choose-a-planning-path/)
- [Documentação BMAD e versão estável](https://docs.bmad-method.org/)
