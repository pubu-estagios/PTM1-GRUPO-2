# PTM1


Faturar+ 📊💰
Sistema de Faturação Completo para Empresas

O Faturar+ é uma plataforma completa para gestão de faturação, ideal para pequenas e médias empresas que desejam organizar suas finanças de forma eficiente. O sistema permite o cadastro de clientes e produtos, emissão e controle de faturas, monitoramento de estoque e análise de relatórios financeiros, tudo em um ambiente intuitivo e seguro.

🚀 Tecnologias Utilizadas
Laravel 11 (com Jetstream + Livewire)
Tailwind CSS (para um design moderno e responsivo)
MySQL (banco de dados relacional)
PDF e Excel Export (para geração de relatórios)
Gmail API (para envio de faturas por e-mail)



✨ Funcionalidades Principais
🔹 Gestão de Clientes
Cadastro completo de clientes, incluindo nome, e-mail, telefone e endereço.
Edição e exclusão de clientes.
Listagem com busca e paginação.


🔹 Cadastro de Produtos
Adição de produtos com nome, descrição, preço e quantidade disponível.
Controle automático de estoque.
Histórico de movimentação de produtos.


🔹 Emissão e Controle de Faturas
Geração de faturas com seleção dinâmica de produtos.
Cálculo automático do valor total com base nos preços e quantidades.
Atualização de estoque ao registrar faturas como pagas.
Opção para baixar faturas em PDF e Excel.
Envio de faturas diretamente pelo e-mail.


🔹 Relatórios Financeiros 📈
Resumo financeiro detalhado.
Gráficos interativos com receita e despesas.
Filtros por período para análise de faturamento.
Relatórios de clientes e produtos vendidos.
Exportação para PDF e Excel.


🔹 Controle de Usuários e Equipes
Multiusuário com permissões baseadas em papéis.
Administração de equipes dentro do sistema.
🛠️ Instalação e Configuração




1️⃣ Requisitos
Antes de instalar, certifique-se de ter instalado:

PHP 8.2+
Composer
Node.js + NPM
MySQL


2️⃣ Clonar o Repositório
bash
Copy
Edit
git clone https://github.com/seuusuario/faturar-plus.git
cd faturar-plus
3️⃣ Instalar Dependências
bash
Copy
Edit
composer install
npm install && npm run dev


4️⃣ Configurar o Banco de Dados
Crie um banco de dados no MySQL e edite o arquivo .env:

env
Copy
Edit
DB_DATABASE=faturar_plus
DB_USERNAME=root
DB_PASSWORD=suasenha
Execute as migrações e seeders:

bash
Copy
Edit
php artisan migrate --seed


5️⃣ Gerar a Chave da Aplicação
bash
Copy
Edit
php artisan key:generate



6️⃣ Iniciar o Servidor
bash
Copy
Edit
php artisan serve
Agora acesse http://127.0.0.1:8000 no seu navegador. 🚀

📩 Envio de E-mails pelo Gmail
Para ativar o envio de faturas por e-mail, configure o Gmail SMTP no .env:

env
Copy
Edit
MAIL_MAILER=smtp
MAIL_HOST=smtp.gmail.com
MAIL_PORT=587
MAIL_USERNAME=seuemail@gmail.com
MAIL_PASSWORD=sua_senha_de_app
MAIL_ENCRYPTION=tls
MAIL_FROM_ADDRESS=seuemail@gmail.com
MAIL_FROM_NAME="Faturar+"


🛡️ Segurança e Autenticação
Login seguro com Laravel Jetstream.
Senhas protegidas com Hashing.
Controle de acesso baseado em permissões.



📜 Licença
Este projeto está sob a MIT License.

Caso precise de ajuda ou queira contribuir, sinta-se à vontade para abrir uma issue ou pull request. 🚀


