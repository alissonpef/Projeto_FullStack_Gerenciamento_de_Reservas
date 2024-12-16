# **Sistema de Gerenciamento de Reservas**

Plataforma completa para a gestão de reservas de recursos do **LabTec**, incluindo computadores, tablets, óculos VR, mesas de trabalho e salas de reunião. Desenvolvido para oferecer uma experiência intuitiva, o sistema permite um controle centralizado e organizado por meio de uma interface web e um banco de dados robusto.

---

## **Sumário**

1. [Visão Geral](#visão-geral)  
2. [Equipe Responsável](#equipe-responsável)  
3. [Principais Funcionalidades](#principais-funcionalidades)  
4. [Tecnologias Utilizadas](#tecnologias-utilizadas)  
5. [Estrutura do Repositório](#estrutura-do-repositório)  
6. [Como Executar](#como-executar)  
7. [Conclusão](#conclusão)

---

## **Visão Geral**

O **Sistema de Gerenciamento de Reservas** foi projetado para atender às necessidades do **LabTec**, permitindo que usuários (alunos, professores e funcionários) possam reservar recursos de forma eficiente e organizada. Cada recurso conta com informações detalhadas e atualizadas, enquanto a administração do sistema é centralizada em um painel que facilita a gestão de permissões e a análise de conflitos de reserva.

---

## **Equipe Responsável**

- **Alisson Pereira Ferreira**  
- **Dennis Paul Paz Lopez**

**Universidade Federal de Santa Catarina (UFSC) – Campus Araranguá**  
Caixa Postal 88.905-120 – Araranguá – SC – Brasil

---

## **Principais Funcionalidades**

1. **Identificação de Usuários**  
   - Cadastro de novos usuários com dados pessoais (nome, sobrenome, CPF, e-mail, senha) e informações adicionais (curso, nacionalidade, data de nascimento, foto de perfil, preferência de tema).
   - Função de recuperação de senha.

2. **Painel Administrativo**  
   - Gerenciamento de usuários: adicionar, remover e editar informações.
   - Definição de permissões e busca filtrada para localizar usuários específicos.

3. **Gerenciamento de Recursos**  
   - **Computadores**: modelo, processador, memória RAM, placa de vídeo, armazenamento e estado de dano.
   - **Kits de Tablets**: tablet associado, presença de caneta, teclado, mouse e estado de dano.
   - **Mesas de Trabalho**: número, presença de monitor, mousepad, fone de ouvido e estado de dano.
   - **Óculos VR**: número, modelo, marca, resolução e estado de dano.
   - **Salas de Reunião**: número, quantidade de mesas/cadeiras, projetor, quadro e estado de dano.
   - **Tablets**: modelo, marca, tamanho de tela, sistema operacional, armazenamento e estado de dano.

4. **Reservas de Recursos**  
   - Agendamento para datas e horários futuros.
   - Prevenção de conflitos de reservas (um mesmo recurso não pode ser reservado simultaneamente por duas pessoas).
   - Visualização completa de todas as reservas no painel administrativo.

---

## **Tecnologias Utilizadas**

- **Python** (Backend e Aplicação Web)
- **PostgreSQL** (Banco de Dados Relacional)
- **pgAdmin** (Administração do Banco de Dados)
- **brModelo** (Modelagem de Banco de Dados)
- **VSCode** (Ambiente de Desenvolvimento)

---

## **Estrutura do Repositório**

```bash
Projeto_Sistema_de_Gerenciamento_de_Reservas
├── apps/                 # Aplicativos principais do sistema
├── config/               # Configurações do projeto
├── requirements/         # Dependências adicionais organizadas
├── static/               # Arquivos estáticos (CSS, JS, imagens)
├── templates/            # Templates HTML para renderização
├── .editorconfig         # Configurações do editor de código
├── .gitattributes        # Configurações do Git
├── .gitignore            # Arquivos e pastas ignorados pelo Git
├── LICENSE               # Licença do projeto
├── Procfile              # Configuração para o Heroku ou serviços semelhantes
├── manage.py             # Script principal para gerenciamento do projeto
├── requirements.txt      # Dependências do Python necessárias para execução
├── runtime.txt           # Versão do ambiente de execução (Heroku, etc.)
└── script.sh             # Script auxiliar para automação de tarefas

```

---

## **Como Executar**

1. **Clonar o Repositório**
   ```bash
    git clone https://github.com/alissonpef/Projeto_FullStack_Controle_de_Acesso_a_Portas.git
   ```

2. **Configurar o Banco de Dados PostgreSQL**
   - Crie um banco de dados chamado `reservas_labtec`.
   - Importe o script `schema.sql` localizado em `Site_Gerencia_de_Reservas/`:
     ```bash
     psql -U seu_usuario -d reservas_labtec -f Site_Gerencia_de_Reservas/schema.sql
     ```

3. **Instalar Dependências**
   - Garanta que você tenha Python instalado.
   - Navegue até a pasta `Site_Gerencia_de_Reservas` e instale os requisitos:
     ```bash
     pip install -r requirements.txt
     ```

4. **Iniciar o Servidor**
   - Ainda na pasta `Site_Gerencia_de_Reservas`, execute:
     ```bash
     python app.py
     ```
   - O sistema estará acessível em:
     ```
     http://localhost:5000
     ```

5. **Acessar e Testar o Sistema**
   - Abra o navegador e acesse `http://localhost:5000`.
   - Utilize as credenciais de teste (se existirem) ou crie um novo usuário para testar as funcionalidades de cadastro, login e reserva.

---

## **Conclusão**

O **Sistema de Gerenciamento de Reservas** oferece uma solução centralizada e segura para administrar os recursos do **LabTec**, permitindo que administradores gerenciem usuários e monitorem reservas, enquanto os usuários usufruem de uma interface intuitiva para realizar agendamentos. Com um backend em Python e um banco de dados PostgreSQL, o sistema está preparado para escalabilidade e futuras integrações. Sugestões ou melhorias podem ser encaminhadas via *issues* ou *pull requests* neste repositório.

---

