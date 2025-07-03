# 🎬 Stream Vibe - Backend Java

Stream Vibe é uma aplicação Java em desenvolvimento que tem como objetivo ser o backend de uma plataforma de streaming. O projeto atualmente implementa as funcionalidades básicas para cadastro e gerenciamento de **filmes**, **usuários** e **endereços**.

## 🧱 Tecnologias Utilizadas

* **Java 17+**
* **Spring Boot**
* **JPA / Hibernate**
* **Banco de Dados Relacional (ex: PostgreSQL ou H2)**
* **Insomnia** (para testes de API REST)

---

## 📁 Estrutura Atual do Projeto

### 📽️ Módulo Filme

Responsável por gerenciar os dados relacionados aos filmes disponíveis na plataforma.

* `Filme`: Entidade principal representando um filme.
* `Genero`: Enum ou classe representando o gênero do filme.
* `DadosCadastroFilme`: DTO para o cadastro de novos filmes.
* `DadosAtualizacaoFilme`: DTO para atualização de filmes existentes.
* `FilmeRepository`: Interface responsável pelas operações com o banco de dados.

### 👤 Módulo Usuário

Gerencia os dados dos usuários da plataforma.

* `Usuario`: Entidade principal representando um usuário.
* `DadosCadastroUsuario`: DTO para o cadastro de novos usuários.
* `UsuarioRepository`: Interface de persistência dos usuários.

### 📍 Módulo Endereço

Relaciona os usuários com seus endereços residenciais.

* `Endereco`: Entidade representando um endereço.
* `DadosCadastroEndereco`: DTO para cadastro de endereço.

---

## 📡 Testes com Insomnia

O projeto está sendo testado via **Insomnia** para consumo das APIs RESTful.

Exemplos de endpoints disponíveis:

* `POST /filmes` – Cadastrar novo filme
* `PUT /filmes/{id}` – Atualizar dados de um filme
* `GET /filmes` – Listar filmes
* `POST /usuarios` – Cadastrar novo usuário
* `GET /usuarios` – Listar usuários
* `POST /enderecos` – Cadastrar endereço

Você pode importar a coleção do Insomnia no próprio aplicativo para facilitar os testes.

---

## 🚀 Como Rodar o Projeto

1. **Clone o repositório**

   ```bash
   git clone https://github.com/seu-usuario/stream-vibe.git
   cd stream-vibe
   ```

2. **Configure o banco de dados**
   Edite o `application.properties` ou `application.yml` com as configurações do seu banco (ex: PostgreSQL ou H2).

3. **Execute o projeto**
   Via sua IDE (IntelliJ, Eclipse) ou terminal:

   ```bash
   ./mvnw spring-boot:run
   ```

4. **Teste os endpoints com Insomnia ou outra ferramenta de API REST.**

---

## 🛠️ Funcionalidades Futuras

* Autenticação com JWT
* Sistema de favoritos
* Catálogo com filtros por gênero, data, avaliação
* Integração com players de vídeo
* Painel administrativo

---

## 📌 Contribuições

Sinta-se à vontade para abrir issues e pull requests!

---

## 📄 Licença

Este projeto está licenciado sob a MIT License.
