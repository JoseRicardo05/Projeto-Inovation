# 🚀 Sistema de Gestão de Projetos e Inovação (SQL)

Este repositório contém o desenvolvimento de um banco de dados relacional completo, focado no gerenciamento de equipes, projetos e tarefas. O projeto foi estruturado para garantir a integridade dos dados e facilitar a extração de informações estratégicas.

## 📌 Contexto do Projeto
O sistema permite cadastrar membros de uma equipe, associá-los a projetos com orçamentos específicos e monitorar o progresso de tarefas individuais, além de gerenciar recursos materiais e técnicos alocados.

## 🛠️ Tecnologias e Habilidades Aplicadas
* [cite_start]**Linguagem:** SQL (MySQL) [cite: 19]
* **Modelagem de Dados:** Criação de tabelas com chaves primárias (`PRIMARY KEY`) e estrangeiras (`FOREIGN KEY`).
* **Relacionamentos:** Implementação de integridade referencial entre as tabelas `Projeto`, `Membro_Equipe` e `Tarefa`.
* [cite_start]**Queries DML/DDL:** Inserção de dados, consultas complexas e manipulação de estrutura. [cite: 19, 20]

## 📊 Estrutura do Banco de Dados
O banco é composto por 6 tabelas integradas:
1. `Membro_Equipe`: Cadastro de colaboradores com cargos e status.
2. `Projeto`: Registro de projetos, orçamentos e definição de gerentes.
3. `Equipe`: Vinculação de equipes aos projetos.
4. `Tarefa`: Controle de demandas, prazos, prioridades e responsáveis.
5. `Recurso`: Gestão de insumos (Humanos, Materiais e Tecnológicos).
6. `Relatorio_Progresso`: Histórico de evolução e problemas enfrentados.

## 🔍 Exemplos de Consultas Praticadas
Durante o projeto, validei diversas formas de extração de dados:

**Busca de membros ativos por cargo:**
```sql
SELECT Nome, Cargo FROM Membro_Equipe WHERE Status_Membro = 'Ativo' AND Cargo LIKE '%Dados%';


