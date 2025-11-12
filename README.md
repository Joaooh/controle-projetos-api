# Proposta 5: Sistema de Controle de Projetos

**Objetivo:** Criar uma API para gerenciamento de projetos, tarefas e responsáveis.
- Projeto
- Tarefa
- Responsavel

**Composição:** Projeto contém várias Tarefas e tem um Responsável

<br>

## Projeto.java
- Contém várias Tarefas
- - Relacionamento @OneToMany com Tarefas
- Tem 1 Responsavel
- - Relacionamento @OneToOne com Responsavel

## Tarefa.java
- Faz parte de vários Projetos (todos os Projetos tem tarefas)
- - @ManyToMany com Projeto?

## Responsavel.java
- Só pode existir 1 Responsavel por Projeto, mas ele pode ser responsável por mais de um Projeto simultaneamente
- - @OneToMany com Projeto?
- Fazer com que Responsavel faça CRUD no Projeto pelo Swagger (criar, ler, atualizar e deletar Projetos o qual é responsável)
