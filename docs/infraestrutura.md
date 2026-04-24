📄 Documento 4 — Camada de Infraestrutura


🎯 Objetivo

Implementar detalhes técnicos e persistência.


🧩 Componentes

🗄️ Banco de Dados

SQLite (local)


📦 Repositórios

AlunoRepository

ProfessorRepository

PagamentoRepository

TurmaRepository


📡 Serviços Externos

Envio de mensagens:

WhatsApp (futuro)

Email (SMTP)


📊 Logs

Registro de erros

Auditoria de operações


🔄 Responsabilidades

Persistir dados

Recuperar dados

Integrar com serviços externos


⚠️ Regras da Camada

Não contém regra de negócio

Implementa interfaces definidas na aplicação/domínio


🔗 Dependências

Bibliotecas externas

Banco de dados
