# Literalura


Este projeto Java foi desenvolvido com o objetivo de exercitar e aprimorar as habilidades de consumo de APIs externas. A API escolhida para este propósito foi a Gutendex, que fornece acesso a uma vasta coleção de livros digitais, permitindo buscas e recuperação de dados de forma programática.

### Tecnologias Utilizadas:

* Java 17: Linguagem de programação principal. 

* Maven: Ferramenta de automação de build e gerenciamento de dependências.

* Jackson: Biblioteca para serialização e desserialização de JSON.

### Instalação

1. Clone o repositório:
   ```bash
   git clone https://github.com/cassiocaiana89/literAlura_DB.git
   cd literAlura_DB
   ```

2. Configure o banco de dados no arquivo `application.properties`:

   ```properties
   spring.datasource.url=jdbc:postgresql://localhost:5432/literAlura
   spring.datasource.username=seu-usuario
   spring.datasource.password=sua-senha
   spring.jpa.hibernate.ddl-auto=update
   spring.jpa.show-sql=true
   ```

3. Para Executar o projeto:

   ```bash
   mvn spring-boot:run
   ```

## Especificações do Projeto:

- No `br.com.alura.literalura`: Pacote principal do projeto.
  - O Pacote `principal`: Contém a classe `Principal`, que gerencia a execução da aplicação.
  - No `model`: Contém as classes de modelo (`Livro`, `Autor`, `LivroDTO`, `AutorDTO`).
  - `repository`: As interfaces de repositório Spring Data JPA.
  - `service`: As classes de serviço (`ConsumoAPI`, `ConverteDados`).

## Autor

Projeto usando a linguagem Java desenvolvido por: [Cássio Caiana](https://github.com/cassiocaiana89)
