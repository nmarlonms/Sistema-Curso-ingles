# Documentação de Requisitos do Sistema

# **Sistema de Gestão para Curso de Inglês**

> **Versão:** 1.1
> 
> 
> **Status:** Em definição
> 
> **Tipo:** Sistema administrativo local
> 

---

# 📚 Sumário

- 1. Introdução
- 2. Objetivo do Sistema
- 3. Escopo do Projeto
- 4. Stakeholders
- 5. Perfis de Usuário
- 6. Requisitos Funcionais
- 7. Requisitos Não Funcionais
- 8. Regras de Negócio
- 9. Módulos do Sistema
- 10. Priorização do MVP
- 11. Casos de Uso
- 12. Estrutura Inicial de Dados
- 13. Decisões Técnicas
- 14. Roadmap
- 15. Pendências

---

# 1. Introdução

Este documento descreve os requisitos do sistema de gestão de um curso de inglês, focado na **administração interna**, com execução local.

O sistema visa organizar e centralizar:

- alunos
- professores
- turmas
- matrículas
- financeiro (receitas e despesas)
- comunicação
- relatórios

---

# 2. Objetivo do Sistema

Fornecer uma solução para:

- controle administrativo completo
- organização financeira
- redução de processos manuais
- suporte à tomada de decisão

---

# 3. Escopo do Projeto

## Incluído

- gestão de alunos
- gestão de professores
- gestão de turmas
- controle de matrículas
- controle financeiro (receber + pagar)
- mensagens
- relatórios
- dashboard

## Não incluído (MVP)

- portal do aluno
- aplicativo mobile
- EAD
- sistema de notas avançado

---

# 4. Stakeholders

## Diretos

- Administração
- Secretaria
- Financeiro
- Coordenação

## Indiretos

- Alunos
- Responsáveis
- Professores

---

# 5. Perfis de Usuário

## Administrador

Acesso total ao sistema.

## Secretaria

Gerenciamento operacional (alunos, turmas, matrículas).

## Financeiro

Controle financeiro (recebimentos e pagamentos).

## Coordenação *(opcional)*

Consulta e acompanhamento pedagógico.

---

# 6. Requisitos Funcionais

---

# RF01 — Autenticação

- RF01.1 Login com usuário e senha
- RF01.2 Logout
- RF01.3 Cadastro de usuários
- RF01.4 Controle de acesso por perfil
- RF01.5 Ativar/desativar usuários

---

# RF02 — Alunos

- RF02.1 Cadastrar aluno
- RF02.2 Editar aluno
- RF02.3 Inativar aluno
- RF02.4 Buscar aluno
- RF02.5 Histórico do aluno

---

# RF03 — Professores

- RF03.1 Cadastrar professor
- RF03.2 Editar professor
- RF03.3 Inativar professor
- RF03.4 Consultar professor
- RF03.5 Vincular professor à turma

---

# RF04 — Turmas

- RF04.1 Cadastrar turma
- RF04.2 Editar turma
- RF04.3 Inativar turma
- RF04.4 Vincular professor
- RF04.5 Vincular alunos
- RF04.6 Transferir alunos

---

# RF05 — Matrículas

- RF05.1 Registrar matrícula
- RF05.2 Vincular aluno à turma
- RF05.3 Alterar status
- RF05.4 Histórico de matrículas

---

# RF06 — Controle Financeiro

## Descrição

Gerenciar receitas (alunos) e despesas (professores).

---

## RF06.1 — Contas a Receber (Alunos)

- RF06.1.1 Criar mensalidades
- RF06.1.2 Gerar cobranças
- RF06.1.3 Registrar pagamentos
- RF06.1.4 Controlar vencimentos
- RF06.1.5 Identificar inadimplência
- RF06.1.6 Histórico financeiro por aluno

---

## RF06.2 — Contas a Pagar (Professores)

- RF06.2.1 Registrar valores a pagar
- RF06.2.2 Registrar pagamento
- RF06.2.3 Consultar pendências
- RF06.2.4 Histórico por professor
- RF06.2.5 Pagamentos por período

---

## RF06.3 — Regras de Remuneração

- RF06.3.1 Definir tipo de pagamento
- RF06.3.2 Valor fixo mensal
- RF06.3.3 Pagamento por turma
- RF06.3.4 Pagamento por aula

---

## RF06.4 — Relatórios Financeiros

- RF06.4.1 Receitas por período
- RF06.4.2 Despesas por período
- RF06.4.3 Inadimplência
- RF06.4.4 Resumo financeiro

---

# RF07 — Mensagens

- RF07.1 Modelos de mensagem
- RF07.2 Envio manual
- RF07.3 Envio em massa
- RF07.4 Histórico
- RF07.5 Mensagens automáticas

---

# RF08 — Relatórios

- RF08.1 Alunos
- RF08.2 Turmas
- RF08.3 Professores
- RF08.4 Financeiro
- RF08.5 Matrículas

---

# RF09 — Dashboard

- RF09.1 Total de alunos
- RF09.2 Turmas ativas
- RF09.3 Pendências financeiras
- RF09.4 Indicadores gerais

---

# RF10 — Auditoria *(opcional)*

- RF10.1 Registrar ações
- RF10.2 Histórico por usuário

---

# 7. Requisitos Não Funcionais

## Ambiente

- Execução local
- Compatível com Windows

## Segurança

- Autenticação obrigatória
- Controle de acesso

## Usabilidade

- Interface simples
- Fácil uso por não técnicos

## Confiabilidade

- Integridade de dados
- Backup

## Manutenção

- Código modular
- Baixo acoplamento

---

# 8. Regras de Negócio

- RN01 Matrícula ativa → aluno ativo
- RN02 Matrícula cancelada → sem cobrança
- RN03 Controle por perfil
- RN04 Inativação ao invés de exclusão
- RN05 Separação entre receitas e despesas
- RN06 Pagamentos de professores devem ser registrados
- RN07 Histórico financeiro não pode ser apagado
- RN08 Controle de capacidade de turma

---

# 9. Módulos do Sistema

- Autenticação
- Alunos
- Professores
- Turmas
- Matrículas
- Financeiro
- Mensagens
- Relatórios
- Dashboard
- Auditoria

---

# 10. MVP

## Incluído

- alunos
- professores
- turmas
- matrículas
- financeiro básico
- relatórios

## Pós-MVP

- mensagens automáticas
- dashboard avançado
- auditoria

---

# 11. Casos de Uso

## UC01 — Cadastrar aluno

## UC02 — Matricular aluno

## UC03 — Registrar pagamento

## UC04 — Registrar pagamento de professor

## UC05 — Enviar mensagem

---

# 12. Estrutura Inicial de Dados

## Aluno

## Professor

## Turma

## Matrícula

---

## Cobrança (Receber)

- aluno_id
- valor
- vencimento
- status

---

## PagamentoProfessor (Pagar)

- professor_id
- valor
- data_pagamento
- status

---

---

# 13. Decisões Técnicas

- Sistema local
- Arquitetura em camadas
- Uso de boas práticas (SOLID)
- Banco local (SQLite ou PostgreSQL)

---

# 14. Roadmap

## Fase 1

Base do sistema

## Fase 2

Financeiro completo

## Fase 3

Automação

## Fase 4

Expansão
