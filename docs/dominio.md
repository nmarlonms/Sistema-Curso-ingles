📄 Documento 3 — Camada de Domínio

🎯 Objetivo

Conter regras de negócio e entidades do sistema.


🧩 Entidades


👤 Aluno

id

nome

responsável

status (ativo/inadimplente)


👨‍🏫 Professor

id

nome

tipo de contrato

valor por aula ou fixo


🏫 Turma

id

nome

professor_id

lista de alunos


💰 Pagamento

id

tipo (aluno/professor)

valor

data

referência (aluno/professor)


📩 Mensagem

id

destinatário

conteúdo

status (enviado/pendente)


📏 Regras de Negócio

Pagamento não pode ter valor negativo

Aluno inadimplente:

quando pagamento estiver atrasado

Professor:

cálculo baseado em contrato

Mensagens automáticas:

disparadas em eventos (ex: atraso)


⚠️ Regras da Camada

Independente de banco ou interface

Código puro (regras)

Alta coesão


🔗 Dependências

Nenhuma (camada mais interna)
