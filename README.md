# MusicConnect

## Índice

- [Sobre o Projeto](#sobre-o-projeto)
- [Funcionalidades](#funcionalidades)
- [Tecnologias Utilizadas](#tecnologias-utilizadas)
- [Banco de Dados](#banco-de-dados)
- [Começando](#começando)
  - [Pré-requisitos](#pré-requisitos)
- [Contato](#contato)
- [Agradecimentos](#agradecimentos)

## Sobre o Projeto

MusicConnect é uma plataforma de rede social inovadora para músicos, desenvolvida como parte do curso de Ciência da Computação na Faculdade Doctum de Caratinga. Este projeto permite que artistas criem perfis, compartilhem sua música, se conectem com outros músicos e fãs, e colaborem em projetos musicais de forma dinâmica e interativa.

O projeto foi desenvolvido com foco nos aspectos operacionais de Sistemas de Gerenciamento de Banco de Dados (SGBD), incluindo transações, controle de concorrência e otimização de consultas. Utilizamos o Laravel como framework PHP principal, MySQL/MariaDB como sistema de gerenciamento de banco de dados, e Tailwind CSS para um frontend moderno e responsivo.

## Funcionalidades

- **Perfis de Usuário**: Registro, autenticação e perfis personalizáveis para músicos.
- **Compartilhamento de Música**: Upload e streaming de arquivos MP3 com player integrado.
- **Rede Social**: Sistema de conexões (seguir/seguidores) entre músicos.
- **Projetos Colaborativos**: Criação e gerenciamento de projetos musicais com múltiplos participantes.
- **Feed de Atividades**: Atualizações em tempo real sobre atividades de conexões e projetos.
- **Mensagens Privadas**: Sistema de mensagens diretas entre usuários.
- **Busca Avançada**: Pesquisa de músicos, músicas e projetos com filtros personalizados.

## Tecnologias Utilizadas

- **Backend**:
  - Laravel 10.x
  - PHP 8.1+
  - MySQL 8.0 / MariaDB 10.5+
  - Redis para cache e filas
  - Laravel Echo e Pusher para funcionalidades em tempo real
  - Laravel Sanctum para autenticação API
- **Frontend**:
  - Tailwind CSS 3.x para estilização
  - Alpine.js para interatividade no cliente
  - Laravel Blade para templates
  - Vite para compilação de assets

## Banco de Dados

A estrutura do banco de dados do MusicConnect é composta pelas seguintes tabelas principais:

- **usuario**
  - `id`: Identificador único do usuário (int)
  - `nome`: Nome completo do usuário (varchar)
  - `nome_usuario`: Nome de usuário (varchar)
  - `senha`: Senha criptografada (varchar)
  - `foto_perfil`: Caminho para a foto de perfil (varchar)
  - `descricao`: Descrição do usuário (text)
  - `created_at`: Data de criação do usuário (timestamp)

- **musica**
  - `id`: Identificador único da música (int)
  - `titulo`: Título da música (varchar)
  - `genero`: Gênero musical (varchar)
  - `data_upload`: Data de upload da música (datetime)
  - `usuario_id`: ID do usuário que enviou a música (int)
  - `arquivo_path`: Caminho do arquivo de música (varchar)

- **projeto_musical**
  - `id`: Identificador único do projeto (int)
  - `nome`: Nome do projeto musical (varchar)
  - `descricao`: Descrição do projeto (text)
  - `criador_id`: ID do usuário criador do projeto (int)
  - `created_at`: Data de criação do projeto (timestamp)

- **feed_atividade**
  - `id`: Identificador único da atividade (int)
  - `usuario_id`: ID do usuário que realizou a atividade (int)
  - `tipo_atividade`: Tipo da atividade (enum: 'upload_musica', 'nova_conexao', 'novo_projeto', 'novo_membro_projeto')
  - `referencia_id`: ID de referência relacionada à atividade (int)

### Diagrama do Banco de Dados
![Diagrama do Banco de Dados](diagrama.jpeg)

## Começando

### Pré-requisitos

- PHP 8.1+
- Composer
- Node.js e npm
- MySQL 8.0 ou MariaDB 10.5+
- (Opcional) Docker e Docker Compose

## Contato

Lucas Marques - lucas@marquesdeveloper.com

Link do Projeto: https://github.com/lucasmarquesfaria/MusicConnect | https://github.com/lucasmarquesfaria/MusicConnect

## Agradecimentos

- Professor M.Sc. Elias Gonçalves pela orientação e suporte
- Faculdades Doctum de Caratinga pela oportunidade de desenvolvimento
