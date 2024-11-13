# UC13 - Executar os Processos de Codificação, Manutenção e Documentação de Aplicativos Computacionais para Desktop

![Foto da atividade feita](automato.png)

## Exercícios - Aula 01

### Objetivo
Esse documento detalha os q fizexercícios da Aula 01, com o objetivo de praticar operações Git, incluindo criação de commits com mensagens detalhadas, reversão de alterações, e manipulação de branches e merges.

---

## Exercício 1 - Criando um Histórico de Commits com Mensagens Detalhadas

**Objetivo**: Aprender a criar um histórico de commits organizado e detalhado usando mensagens de commit.

**Passos**:

1. Criei uma nova pasta chamada(mkdir) `git-historico`.
2. Inicializei essa pasta como um repositório Git:
   ```bash
   git init
   ```
3. Criei três arquivos diferentes(vscode):
   - `notas.txt`: Inclua algum conteúdo relevante.
   - `resumo.md`: Adicione um resumo ou descrição.
   - `tarefa.txt`: Descreva uma tarefa ou objetivo.

4. Adicionei o commit de cada arquivo separadamente, usando mensagens de commit detalhadas que expliquem o conteúdo e a intenção de cada mudança:
   ```bash
   git add notas.txt
   git commit -m "Adicionando notas sobre o projeto no arquivo notas.txt"

   git add resumo.md
   git commit -m "Adicionando resumo do projeto no arquivo resumo.md"

   git add tarefa.txt
   git commit -m "Descrevendo a tarefa principal no arquivo tarefa.txt"
   ```
5. Exibindo o histórico de commits para verificar as mensagens:
   ```bash
   git log
   ```

---

## Exercício 2: Desfazendo Alterações com `git reset` e `git restore`

**Objetivo**: Pratiquei a reversão de alterações não commitadas e commitadas no repositório Git.

**Passos**:

1. Criei uma nova pasta chamada `projeto-reversao`.
2. Comecei essa pasta como um repositório Git:
   ```bash
   git init
   ```
3. Criei um arquivo `experimento.txt` e fiz o conteúdo inicial.
4. Adicionei e faça o commit do arquivo:
   ```bash
   git add experimento.txt
   git commit -m "Adiciona conteúdo inicial no experimento.txt"
   ```
5. Modifiquei o arquivo `experimento.txt` (sem fazer commit) e usei `git restore` para desfazer as mudanças não commitadas:
   ```bash
   git restore experimento.txt
   ```
6. Fiz mais uma modificação no arquivo e, fiz commit dessa vez:
   ```bash
   echo "Nova alteração" >> experimento.txt
   git add experimento.txt
   git commit -m "Adicionando nova alteração no experimento.txt"
   ```
7. Use `git reset --hard` para reverção o último commit:
   ```bash
   git reset --hard HEAD~1
   

---

