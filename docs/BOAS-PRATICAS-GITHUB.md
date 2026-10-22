# Boas práticas de GitHub para o desafio

Está começando? Use o [cookbook de alunos e mentores](../COOKBOOK-GITHUB.md), com os cliques de envio, revisão e aprovação.

## 1. Um repositório por aluno ou dupla

Use o repositório de referência como modelo e mantenha o projeto em um repositório individual. Isso separa as entregas e deixa a avaliação mais clara. Se o repositório for privado, convide o instrutor como colaborador antes da primeira entrega.

### Configuração inicial do repositório

- Habilite **Template repository** nas configurações do repositório de referência.
- Para cada aluno, crie uma cópia individual e defina a visibilidade combinada com a turma.
- Em cada repositório privado, convide os dois mentores e confirme que aceitaram. Em conta pessoal, colaboradores possuem escrita; em organizações, a coordenação pode ajustar papéis mais específicos. Não presuma que colaboradores e proteções foram copiados do template.
- Mantenha a branch `main` como branch padrão. Se disponível, exija Pull Request para integrar mudanças; em turmas pequenas, a revisão do instrutor no PR já serve como controle mínimo.
- Não publique o repositório do aluno se houver informação que não deve ficar pública.

## 2. Proteja a branch principal

- Use `main` como versão que deve sempre funcionar.
- Evite editar diretamente na `main`.
- Faça cada mudança em uma branch curta.
- Abra um Pull Request (PR) para integrar a mudança.
- Revise os comentários e atualize o PR antes de pedir aprovação.

## 3. Nomes de branches

Use nomes curtos que expliquem o trabalho:

```text
docs/pre-projeto
feat/login-perfis
feat/cadastro-contatos
feat/pipeline-oportunidades
fix/validacao-email
```

## 4. Commits pequenos e claros

Faça commits quando concluir uma alteração lógica. Exemplos:

```text
docs: registra problema e escopo do CRM
feat: permite cadastrar contatos
fix: bloqueia operador de editar usuário
test: verifica permissões do operador
```

Evite mensagens como `mudanças`, `final`, `versão nova` ou commits gigantes com todo o projeto.

## 5. Issues para acompanhar o trabalho

Abra um Issue para cada marco e, depois, para as histórias de usuário. Um Issue deve responder: o que será feito, por que, como saberemos que terminou e quais são as dependências. Associe o PR ao Issue, por exemplo `Closes #12`.

## 6. Pull Requests para avaliação

Um PR deve conter uma alteração pequena e revisável. Na descrição, informe:

- Issue relacionado;
- o que mudou;
- como testar;
- critérios de aceite atendidos;
- limitações ou pontos não verificados;
- captura de tela ou gravação curta quando a mudança for visual.

Marque o PR como pronto quando os arquivos e as instruções estiverem preparados para a revisão do mentor. Use Draft enquanto ainda estiver trabalhando. Responda aos comentários no próprio PR e peça nova revisão após os ajustes.

## 7. Segredos e dados pessoais

- Nunca envie `.env`, senhas, tokens, chaves de API ou certificados para o GitHub.
- Inclua `.env.example` com nomes das variáveis e valores vazios/de exemplo, sem credenciais reais.
- Confira `git status` e os arquivos do PR antes de enviar.
- Use nomes, e-mails e empresas fictícios nos dados de demonstração.
- Se um segredo for publicado por engano, remova-o do serviço onde ele foi criado e gere outro. Apagar o arquivo em um commit posterior não invalida o segredo exposto.

## 8. README e reprodutibilidade

O README do aplicativo deve permitir que outra pessoa o rode sem adivinhar:

1. pré-requisitos;
2. instalação;
3. variáveis de ambiente necessárias, sem valores secretos;
4. preparação do banco de dados;
5. inicialização;
6. execução de testes;
7. contas/dados de demonstração fictícios;
8. limitações conhecidas.

## 9. Histórico e avaliação

O histórico do GitHub é parte da entrega. Mantenha os Issues, branches, commits e PRs usados durante o projeto. Não reescreva o histórico para esconder decisões ou concentrar tudo em um único commit final.

Para facilitar a avaliação, use títulos claros como **Marco 1 — Pré-projeto**, **Marco 2 — Plano BMAD** e **Entrega final — CRM**. No PR de cada marco, inclua os links dos artefatos e marque o instrutor como revisor.

## 10. Comandos básicos

```bash
# Conferir arquivos modificados
git status

# Criar e trocar para uma branch
git switch -c feat/cadastro-contatos

# Preparar arquivos e salvar um commit
git add .
git commit -m "feat: permite cadastrar contatos"

# Enviar a branch para o GitHub
git push -u origin feat/cadastro-contatos

# Atualizar a main local antes de iniciar outra tarefa
git switch main
git pull
```

Antes de usar `git add .`, confira o `git status` para não incluir `.env`, arquivos temporários ou dados pessoais.
