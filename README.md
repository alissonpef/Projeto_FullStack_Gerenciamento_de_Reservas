# Sistema de Gerenciamento de Reservas

## Descrição

O objetivo geral deste sistema de gerenciamento de reservas do LabTec é fornecer uma plataforma robusta onde os usuários possam acessar e reservar uma variedade de recursos disponíveis no laboratório, como computadores, tablets, óculos VR, mesas de trabalho e mesas de reunião. O sistema visa oferecer uma experiência intuitiva e eficiente, permitindo aos usuários explorar e reservar os recursos conforme suas necessidades, garantindo também a gestão eficiente e organizada dos dados por meio de um banco de dados bem estruturado.

## Integrantes do Projeto
- **Alisson Pereira Ferreira**
- **Dennis Paul Paz Lopez**

**Universidade Federal de Santa Catarina (UFSC) – Campus Araranguá**  
Caixa Postal 88.905-120 – Araranguá – SC – Brasil

## Funcionalidades

### Identificação dos Usuários

Cada usuário do sistema terá as seguintes informações armazenadas no banco de dados:

- 📧 **Dados Pessoais**: e-mail, senha, nome, sobrenome, CPF.
- 📝 **Informações Adicionais**: curso, nacionalidade, data de nascimento, foto de perfil e preferência pelo modo escuro ou claro.

Os usuários serão criados por meio de um formulário simples com campos para nome, e-mail e senha. Haverá uma opção para recuperação de senha caso o usuário esqueça a senha.

### Gestão Centralizada via Painel Administrativo

Os administradores terão acesso a um Painel Administrativo que permitirá:

- 👤 **Gerenciamento de Usuários**: adicionar, remover, editar informações e gerenciar permissões dos usuários.
- 🔍 **Busca Filtrada**: realizar buscas filtradas para encontrar usuários específicos ou grupos de usuários com base em diferentes critérios.

### Armazenamento Detalhado dos Recursos Disponíveis

O sistema armazenará informações detalhadas sobre os seguintes recursos:

- 💻 **Computadores**: número, processador, memória RAM, placa de vídeo, armazenamento, sistemas operacionais, disponibilidade de fone de ouvido e estado de dano.
- 📱 **Kits de Tablets**: presença de caneta, teclado, mouse, estado de dano, e referência ao tablet associado.
- 🪑 **Mesas de Trabalho**: número, presença de monitor, mousepad, fone de ouvido, e estado de dano.
- 🕶️ **Óculos VR**: número, modelo, marca, resolução, e estado de dano.
- 🏢 **Salas de Reunião**: número, quantidade de mesas e cadeiras, presença de projetor e quadro, e estado de dano.
- 📲 **Tablets**: número, modelo, marca, tamanho da tela, sistema operacional, armazenamento, e estado de dano.

### Gerenciamento de Reservas pelos Usuários

Os usuários poderão reservar os recursos mencionados acima para um horário específico em um determinado dia, com as seguintes regras para reservar:

- 🗓️ **Reservas Futuras**: Reservas só podem ser feitas para o presente e futuro, nunca para datas passadas.
- 🚫 **Conflito de Reservas**: Um recurso não pode ser reservado por mais de uma pessoa ao mesmo tempo.

Os administradores poderão visualizar todas as reservas realizadas, garantindo um gerenciamento eficiente e a disponibilidade adequada dos recursos.

## Componentes Utilizados

- 💻 **VSCode**: Ambiente de desenvolvimento utilizado para a codificação do sistema.
- 🐘 **PostgreSQL**: Banco de dados relacional utilizado para armazenar os dados do sistema.
- 🖥️ **pgAdmin**: Interface gráfica para gerenciamento e administração do PostgreSQL.
- 🧑‍💻 **brModelo**: Ferramenta de modelagem de banco de dados usada para criar o diagrama relacional.

## Modelagem Conceitual

![image](https://github.com/user-attachments/assets/f240b36e-814c-4292-8ed5-3c2f9a0fbeef)

## Modelagem Lógica

![image](https://github.com/user-attachments/assets/0055af30-4e02-4f37-87d2-6eb70d4362ae)

## **Resumindo:**  

Em resumo, o sistema inclui o cadastro e armazenamento de dados dos usuários, a gestão via Painel Administrativo, armazenamento detalhado dos recursos disponíveis e o gerenciamento de reservas pelos usuários. O sistema foi implementado usando um modelo relacional no banco de dados PostgreSQL, garantindo uma base flexível para o desenvolvimento do sistema, permitindo a capacidade de expansão futura.
