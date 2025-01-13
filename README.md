# LiterAlura - Sistema de Gerenciamento de Livros e Autores

## Descrição
LiterAlura é uma aplicação que permite buscar, registrar e gerenciar informações sobre livros e autores. Utiliza uma API externa (“GutenDex”) para buscar dados de livros e registra-los em um banco de dados local, permitindo consultas e filtragens personalizadas.

## Funcionalidades

### 1. Buscar livro por título
- Busca livros em uma API externa com base no título informado.
- Registra o livro e o autor correspondente no banco de dados, caso ainda não estejam cadastrados.
- Exibe informações detalhadas do livro, como:
  - Título
  - Idioma
  - Autor
  - Número de downloads

### 2. Listar livros registrados
- Mostra todos os livros armazenados no banco de dados com:
  - Título
  - Autor
  - Idioma
  - Número de downloads

### 3. Listar autores registrados
- Exibe todos os autores registrados no banco de dados, incluindo:
  - Nome
  - Data de nascimento
  - Data de falecimento (se aplicável)
  - Livros associados

### 4. Listar autores vivos em um ano específico
- Permite buscar autores que estavam vivos em um ano informado pelo usuário.

### 5. Listar livros por idioma
- Filtra livros registrados com base no idioma especificado (ex.: “es”, “en”, “fr”, “pt”).

### 6. Sair
- Encerra a execução do programa.

## Tecnologias Utilizadas
- **Java 17**: Linguagem principal.
- **Spring Framework**: Injeção de dependências e gestão dos serviços.
- **Hibernate/JPA**: Mapeamento objeto-relacional para interagir com o banco de dados.
- **Jakarta Persistence API (JPA)**: Para definição de entidades.
- **Gson**: Conversão de JSON para objetos Java e vice-versa.
- **API GutenDex**: Fonte de dados externa para busca de livros.

## API Externa
**Base URL da API GutenDex**: `https://gutendex.com/books/`
- Permite buscar livros por título utilizando o endpoint `?search=<titulo>`.

## Exemplo de Uso
- **Busca de Livro**:
  1. Informe o título do livro no menu.
  2. O sistema buscará os dados na API externa e exibirá informações detalhadas.

- **Listagem de Livros Registrados**:
  1. Escolha a opção correspondente no menu.
  2. Será exibida uma lista de todos os livros cadastrados no sistema.

