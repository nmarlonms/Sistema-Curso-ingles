📄 Documento 2 — Camada de Aplicação

🎯 Objetivo

Orquestrar os casos de uso do sistema.

🧩 Casos de Uso (Serviços)

👤 Aluno

CadastrarAluno

AtualizarAluno

ListarAlunos

👨‍🏫 Professor

CadastrarProfessor

AtualizarProfessor

ListarProfessores

💰 Financeiro

RegistrarPagamentoAluno

RegistrarPagamentoProfessor

GerarRelatorioFinanceiro

📢 Comunicação

EnviarMensagemManual

ProcessarMensagensAutomaticas

🔄 Fluxo padrão de um serviço

Recebe dados da UI

Valida entrada

Chama regras do domínio

Persiste via repositório

Retorna resposta

⚠️ Regras da Camada

Não implementa regras de negócio complexas

Não acessa banco diretamente

Usa interfaces de repositório

🔗 Dependências

Camada de Domínio

Interfaces da Infraestrutura
