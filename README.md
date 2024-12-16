# Sistema de Gerenciamento de Reservas

## Descrição

O objetivo geral deste sistema de gerenciamento de reservas do **LabTec** é fornecer uma plataforma robusta onde os usuários possam acessar e reservar uma variedade de recursos disponíveis no laboratório, como computadores, tablets, óculos VR, mesas de trabalho e mesas de reunião. O sistema visa oferecer uma experiência intuitiva e eficiente, permitindo aos usuários explorar e reservar os recursos conforme suas necessidades, garantindo também a gestão eficiente e organizada dos dados por meio de um banco de dados bem estruturado.

---

## 👥 Integrantes do Projeto

- **Alisson Pereira Ferreira**
- **Dennis Paul Paz Lopez**

**Universidade Federal de Santa Catarina (UFSC) – Campus Araranguá**  
Caixa Postal 88.905-120 – Araranguá – SC – Brasil

---

## ⚙️ Funcionalidades

### Identificação dos Usuários

Cada usuário do sistema terá as seguintes informações armazenadas no banco de dados:

- 📧 **Dados Pessoais**: e-mail, senha, nome, sobrenome, CPF.
- 📝 **Informações Adicionais**: curso, nacionalidade, data de nascimento, foto de perfil e preferência pelo modo escuro ou claro.

Os usuários serão criados por meio de um formulário simples com campos para nome, e-mail e senha. Haverá uma opção para recuperação de senha caso o usuário esqueça a senha.

### Gestão Centralizada via Painel Administrativo

Os administradores terão acesso a um **Painel Administrativo** que permitirá:

- 👤 **Gerenciamento de Usuários**: adicionar, remover, editar informações e gerenciar permissões dos usuários.
- 🔍 **Busca Filtrada**: realizar buscas filtradas para encontrar usuários específicos ou grupos de usuários com base em diferentes critérios.

### Armazenamento Detalhado dos Recursos Disponíveis

O sistema armazenará informações detalhadas sobre os seguintes recursos:

- 💻 **Computadores**: número, processador, memória RAM, placa de vídeo, armazenamento, sistemas operacionais, disponibilidade de fone de ouvido e estado de dano.
- 📱 **Kits de Tablets**: presença de caneta, teclado, mouse, estado de dano e referência ao tablet associado.
- 🪑 **Mesas de Trabalho**: número, presença de monitor, mousepad, fone de ouvido e estado de dano.
- 🕶️ **Óculos VR**: número, modelo, marca, resolução e estado de dano.
- 🏢 **Salas de Reunião**: número, quantidade de mesas e cadeiras, presença de projetor e quadro, e estado de dano.
- 📲 **Tablets**: número, modelo, marca, tamanho da tela, sistema operacional, armazenamento e estado de dano.

### Gerenciamento de Reservas pelos Usuários

Os usuários poderão reservar os recursos mencionados acima para um horário específico em um determinado dia, com as seguintes regras para reservar:

- 🗓️ **Reservas Futuras**: Reservas só podem ser feitas para o presente e futuro, nunca para datas passadas.
- 🚫 **Conflito de Reservas**: Um recurso não pode ser reservado por mais de uma pessoa ao mesmo tempo.

Os administradores poderão visualizar todas as reservas realizadas, garantindo um gerenciamento eficiente e a disponibilidade adequada dos recursos.

---

## 🛠️ Componentes Utilizados

- 💻 **VSCode**: Ambiente de desenvolvimento utilizado para a codificação do sistema.
- 🐘 **PostgreSQL**: Banco de dados relacional utilizado para armazenar os dados do sistema.
- 🖥️ **pgAdmin**: Interface gráfica para gerenciamento e administração do PostgreSQL.
- 🧑‍💻 **brModelo**: Ferramenta de modelagem de banco de dados usada para criar o diagrama relacional.

---

## 🛠️ Como Executar

### 1. Clonar o Repositório

```bash
git clone https://github.com/alissonpef/Projeto_Sistema_de_Gerenciamento_de_Reservas.git
```

### 2. Configurar o Banco de Dados PostgreSQL

- Crie um banco de dados chamado `reservas_labtec` no PostgreSQL.
- Utilize o arquivo `schema.sql` localizado na pasta `Site_Gerencia_de_Reservas` para configurar as tabelas:

```bash
psql -U seu_usuario -d reservas_labtec -f Site_Gerencia_de_Reservas/schema.sql
```

### 3. Configurar o Ambiente de Desenvolvimento

Certifique-se de ter o Python instalado e configure as dependências do servidor:

```bash
pip install -r requirements.txt
```

### 4. Iniciar o Servidor

Navegue até o diretório `Site_Gerencia_de_Reservas` e execute o servidor:

```bash
python app.py
```

### 5. Acessar o Sistema

Abra o navegador e acesse o sistema em:

```
http://localhost:5000
```

---

## 🌟 Resumindo

O **Sistema de Gerenciamento de Reservas** oferece uma solução completa para a gestão de recursos do **LabTec**, com funcionalidades de cadastro de usuários, painel administrativo, armazenamento detalhado de recursos e gerenciamento de reservas. Implementado com um banco de dados PostgreSQL e uma interface eficiente, o sistema é intuitivo e flexível para atender às necessidades de expansão futura.

---

