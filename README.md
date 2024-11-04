# MusicConnect

MusicConnect é uma rede social para músicos, desenvolvida como parte do curso de Ciência da Computação na Faculdade Doctum de Caratinga. Esta plataforma permite que artistas criem perfis, compartilhem sua música, se conectem com outros músicos e fãs, e colaborem em projetos musicais.

## Visão Geral

O projeto MusicConnect foi desenvolvido com foco nos aspectos operacionais de SGBD, incluindo transações, controle de concorrência e otimização de consultas. A aplicação utiliza PHP para o backend e MySQL/MariaDB como sistema de gerenciamento de banco de dados.

### Funcionalidades Principais

- Registro e perfis de usuários
- Compartilhamento de música (upload de arquivos MP3)
- Conexões entre músicos
- Criação e gerenciamento de projetos musicais colaborativos
- Feed de atividades para acompanhar atualizações de amigos e projetos

## Tecnologias Utilizadas

- PHP 7.4+
- MySQL 8.0 / MariaDB 10.5+
- HTML5, CSS3, JavaScript
- [Outras bibliotecas ou frameworks utilizados]

## Estrutura do Banco de Dados

O banco de dados do MusicConnect consiste nas seguintes tabelas principais:

- `usuario`: Armazena informações dos usuários
- `musica`: Contém detalhes das músicas enviadas pelos usuários
- `conexao`: Registra as conexões entre os usuários
- `projeto_musical`: Armazena informações sobre projetos musicais
- `membro_projeto`: Associa usuários a projetos musicais
- `feed_atividade`: Registra as atividades dos usuários na plataforma


## Agradecimentos

- Professor M.Sc. Elias Gonçalves
- Faculdades Doctum de Caratinga
- [Outros agradecimentos relevantes]
