# Projeto: Gerenciador de Tarefas v2.0

## 1. Visão Geral

Este é um projeto de um Gerenciador de Tarefas via terminal, desenvolvido em Python. A base do projeto oferece funcionalidades para adicionar, listar, concluir e remover tarefas. O objetivo deste trabalho é estender a funcionalidade do sistema e demonstrar um fluxo de trabalho de desenvolvimento profissional utilizando Git e GitHub.

## 2. Configuração Inicial

1.  **Fork:** Realize um fork deste repositório para a sua conta pessoal no GitHub.
2.  **Clone:** Clone o repositório que você criou (o seu fork) para o seu ambiente de desenvolvimento local.
    ```bash
    git clone [https://github.com/SEU-USUARIO/NOME-DO-REPOSITORIO.git](https://github.com/SEU-USUARIO/NOME-DO-REPOSITORIO.git)
    ```

## 3. Especificações da Tarefa

Você deve implementar as **duas** novas funcionalidades descritas abaixo.

### Funcionalidade 1: Prioridade de Tarefas

* **Estrutura de Dados:** A estrutura de dados de cada tarefa deve ser alterada para incluir um campo `prioridade`.
* **Adicionar Tarefa:** A função de adição deve ser modificada para solicitar ao usuário um nível de prioridade (`Alta`, `Média`, `Baixa`). Uma entrada inválida deve resultar na prioridade padrão `Baixa`.
* **Listar Tarefas:** A função de listagem deve ser atualizada para exibir a prioridade de cada tarefa.

### Funcionalidade 2: Edição de Descrição da Tarefa

* **Menu:** Uma nova opção para "Editar Tarefa" deve ser adicionada ao menu principal.
* **Implementação:** Deve ser criada uma função que permita ao usuário:
    1.  Selecionar uma tarefa existente pelo seu índice.
    2.  Visualizar a descrição atual.
    3.  Inserir uma nova descrição para substituí-la.
* **Feedback:** O sistema deve informar ao usuário se a operação foi bem-sucedida.

## 4. Requisitos de Entrega e Fluxo de Trabalho

A avaliação levará em conta a organização do seu repositório e o uso correto das ferramentas.

* **README.md:** Este arquivo deve ser atualizado com a seção "Minhas Contribuições" devidamente preenchida.
* **`.gitignore`:** O repositório precisa conter um arquivo `.gitignore` configurado adequadamente para projetos Python, ignorando arquivos e pastas como `__pycache__` e `venv/`.
* **Fluxo com Branches:** Cada uma das duas funcionalidades deve ser desenvolvida em uma *feature branch* separada (ex: `feature/task-priority` e `feature/edit-task-description`). Após a finalização, cada branch deve ser mesclada (`merge`) de volta à branch `main`.
* **Histórico de Commits:** É exigido um histórico com um mínimo de **8 a 10 commits atômicos**. As mensagens de commit devem ser claras e refletir o trabalho realizado em cada etapa.

## 5. Critérios de Avaliação

* **README:** Clareza e detalhamento da seção "Minhas Contribuições".
* **Git:** Qualidade das mensagens de commit e demonstração do fluxo de trabalho com branches e merges.
* **Funcionalidade:** Implementação correta e funcional das modificações solicitadas.
* **Código:** Legibilidade, organização e qualidade geral do código implementado.

---

## (Template para o Aluno)


* **Nome:** Erik da Silva Xavier  
* **GitHub:** [https://github.com/Erik-Xavier](https://github.com/Erik-Xavier)

---

### Modificação 1: Prioridade de Tarefas

**Lógica Implementada:**
- A estrutura da tarefa foi expandida com o campo `"prioridade"` (Alta, Média ou Baixa).
- O usuário escolhe a prioridade ao adicionar uma nova tarefa.
- Se a entrada for inválida, a prioridade padrão será "Baixa".
- A função `listar_tarefas()` foi atualizada para exibir a prioridade de cada item.

**Como Testar:**
1. Escolha a opção **1. Adicionar Tarefa** no menu.
2. Digite uma descrição.
3. Escolha um número de 1 a 3 para definir a prioridade.
4. Liste as tarefas (opção 2) e verifique se a prioridade aparece corretamente.

---

### Modificação 2: Editar Descrição da Tarefa

**Lógica Implementada:**
- Adicionada a opção **5. Editar Descrição da Tarefa** ao menu.
- Criada a função `editar_descricao_tarefa()` que permite alterar a descrição de uma tarefa existente.
- O sistema exibe a descrição atual e solicita uma nova, impedindo que o campo fique vazio.

**Como Testar:**
1. Escolha a opção **5. Editar Descrição da Tarefa** no menu.
2. Digite o número da tarefa que deseja editar.
3. Informe a nova descrição quando solicitado.
4. Liste as tarefas para verificar se a mudança foi salva.
