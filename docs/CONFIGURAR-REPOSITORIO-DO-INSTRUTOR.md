# Publicar o repositório de referência no GitHub

Este pacote já é um repositório Git local e contém o primeiro commit. Os passos abaixo criam o repositório central do desafio; os alunos depois criam uma cópia própria a partir dele.

## 1. Criar o repositório remoto

1. Entre na conta GitHub que será proprietária do material.
2. Abra [github.com/new](https://github.com/new).
3. Use o nome `desafio-crm-zero-to-hero`.
4. Escolha **Public** para que os alunos possam acessar e copiar o material. O repositório contém somente enunciado, instruções e modelos; não envie trabalhos de alunos ou dados privados para ele.
5. **Não** marque as opções de adicionar README, `.gitignore` ou licença, pois esses arquivos já existem no repositório local.
6. Crie o repositório.

## 2. Enviar os arquivos locais

No terminal, dentro da pasta `desafio-crm-zero-to-hero`, conecte o repositório local ao endereço criado e envie a branch `main`:

```bash
git remote add origin https://github.com/SEU-USUARIO/desafio-crm-zero-to-hero.git
git push -u origin main
```

Substitua `SEU-USUARIO` pelo proprietário real do repositório. Confirme no navegador que `README.md`, `DESAFIO.md` e `docs/` aparecem.

## 3. Habilitar como modelo

No repositório remoto, abra **Settings → General → Template repository** e habilite a opção. Isso permite que cada estudante crie uma cópia independente com **Use this template → Create a new repository**.

## 4. Configurar a avaliação individual

- Oriente cada aluno a criar seu próprio repositório a partir do modelo.
- O aluno escolhe a visibilidade combinada com a turma. Para avaliação privada, adiciona o instrutor em **Settings → Collaborators**.
- O aluno usa Issues para marcos/histórias e Pull Requests para as entregas.
- O instrutor registra o resultado do Marco 1 e a rubrica final nos PRs do próprio aluno.
- Mantenha trabalhos de alunos fora do repositório público de referência.

Se a turma já utiliza GitHub Classroom, o instrutor pode adaptar o repositório de referência como base da atividade e usar os repositórios individuais gerados pela sala.
