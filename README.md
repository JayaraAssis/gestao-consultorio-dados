🏥 Gestão de Consultório — Projeto de Banco de Dados
📊 Portfólio — 2025/2

Repositório dedicado ao desenvolvimento de um sistema de gestão de dados de consultório médico, com foco na qualidade e integridade das informações.
O projeto simula o fluxo de uma clínica: cadastro de consultórios, médicos, pacientes e consultas — tudo com regras de negócio aplicadas no PL/SQL.

✅ Objetivo do Projeto

📌 Desenvolver um banco de dados para gestão de saúde que:

-Garanta integridade e confiabilidade dos dados

-Implemente validações reais de CPF e CNPJ (com dígito verificador)

-Utilize procedures, triggers e funções para regras de negócio

-Permita geração de relatórios analíticos para apoio à gestão

🧱 Arquitetura do Banco

🛠 Modelo utilizado: Monólito

Uma única instância de banco, pois até o momento o escopo é de uso pessoal para portfólio, sem necessidade de escalabilidade.

📌 Entidades principais:

Entidade	Função
-CONSULTORIO	Identificação do estabelecimento
-MEDICOS	Profissionais que atendem
-PACIENTES	Clientes do serviço médico
-CONSULTAS	Histórico de atendimentos e faturamento

**Regras de Negócio Implementadas **
-Validação	Onde acontece
-CPF válido (dígito verificador)	Function + Trigger
-CNPJ válido	Function + Trigger
-Evitar duplicidade de CPF e CNPJ	Procedures
-Paciente e Médico devem pertencer ao consultório informado	Procedure CONSULTAS
-Datas e valores válidos	Procedures
-Integridade referencial	FKs

✅ Ninguém consegue inserir dados inválidos diretamente na tabela
🔐 O banco está blindado contra erros humanos

📂 Estrutura do Repositório
gestao-consultorio-dados/
│
├── sql/
│   ├── 01-create-tables.sql
│   ├── 02-functions.sql
│   ├── 03-triggers.sql
│   ├── 04-procedures.sql
│   ├── 05-test-data.sql
│   └── 06-analytics-queries.sql
│
├── docs/
│   └── diagrama-er.png (em breve)
│
└── README.md

🔍 Consultas Analíticas (Business Insights)

Exemplos reais já implementados ✅

- Faturamento por mês

- Médico com mais atendimentos

- Pacientes que mais utilizam o serviço

- Consultas por especialidade

- Consultas por período

➡ códigos completos estão em 06-analytics-queries.sql ✅
➡ prints dos resultados serão adicionados em breve ✅
➡ Diagrama Entidade Relacionamento (docs/diagrama-er.png) ✅

** Como Executar o Projeto **
✅ No Oracle Live SQL

1️⃣ Acesse https://livesql.oracle.com

2️⃣ Execute os arquivos na ordem:

01-create-tables.sql
02-functions.sql
03-triggers.sql
04-procedures.sql
05-test-data.sql (opcional)
06-analytics-queries.sql


# IMPORTANTE:

As triggers e FKs impedirão inserções inválidas — comportamento esperado ✅

** Tecnologias Utilizadas **
-Tecnologia	Função
-Oracle Database	Armazenamento e regras
-PL/SQL	Procedures e triggers
-SQL Developer / Oracle Live SQL	Execução e testes
-Git & GitHub	Controle de versão e portfólio
👩‍💻 Desenvolvido por

Jayara Cristina Assis dos Santos Silva
Estudante de Tecnologia com foco em Banco de Dados
📆 Projeto Pessoal — Portfólio 2025/2

🚀 Próximas melhorias

Inserção de mais dados para análises avançadas

Diagrama ER completo e estilizado (em breve)

Views para simplificar relatórios

Scripts automatizados de carga

⭐ Se gostou do projeto, não esqueça de marcar com uma estrela no GitHub!
Ajuda muito o meu crescimento na área! 

