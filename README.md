
```markdown
# Cadastro de Usuário

Projeto desenvolvido em Java com Spring Boot, utilizando Maven como ferramenta de build. Esta aplicação tem como objetivo **gerenciar o cadastro de usuários**, permitindo criar, buscar, atualizar e deletar usuários por meio de uma API RESTful.

---

## 📖 Sumário

- [Descrição](#descrição)
- [Tecnologias Utilizadas](#tecnologias-utilizadas)
- [Pré-requisitos](#pré-requisitos)
- [Configuração do Ambiente](#configuração-do-ambiente)
- [Como Executar a Aplicação](#como-executar-a-aplicação)
- [Executando os Testes](#executando-os-testes)
- [Estrutura do Projeto](#estrutura-do-projeto)
- [Configurações e Perfis](#configurações-e-perfis)
- [Ambiente de Produção](#ambiente-de-produção)
- [Contribuição](#contribuição)

---

## 📌 Descrição

Este projeto é uma aplicação backend que expõe uma API RESTful para **gerenciamento de usuários**. O sistema foi construído com foco em **boas práticas de desenvolvimento**, como separação de camadas (controller, service, repository).

---

## 🚀 Tecnologias Utilizadas

- **Java 17**
- **Spring Boot 3.x**
    - Spring Web
    - Spring Data JPA
- **Maven 3.8+**
- **Banco de Dados:** 
    - H2
- **Lombok**

---

## ✅ Pré-requisitos

Antes de iniciar, você precisará ter os seguintes softwares instalados:

- [Java JDK 17 ou superior](https://www.oracle.com/java/technologies/javase/jdk17-archive-downloads.html)
- [Apache Maven 3.8+](https://maven.apache.org/download.cgi)
- [Git](https://git-scm.com/)
- IDE de sua preferência (IntelliJ IDEA, VS Code, Eclipse etc.)

---

## ⚙️ Configuração do Ambiente

1. Clone o repositório:
   ```bash
   git clone https://github.com/linconvinicius/cadastro-usuario.git
   cd cadastro-usuario
   ```

2. Configure o arquivo `src/main/resources/application.properties` com as credenciais do seu banco de dados:
   ```
   spring.datasource.url=/usuario
   spring.datasource.username=seu_usuario
   spring.datasource.password=sua_senha
   ```

---

## ▶️ Como Executar a Aplicação

Execute o comando abaixo na raiz do projeto:

```bash
mvn spring-boot:run
```

A aplicação estará disponível em: [http://localhost:8080](http://localhost:8080)

---

## 🧪 Executando os Testes

Para rodar os testes automatizados:

```bash
mvn test
```

---

## 📁 Estrutura do Projeto

```
src/
 └── main/
     ├── java/
     │    └── com/
     │         └── lvtech/
     │              └── cadastro_usuario/
     │                   ├── controller/
     │                   ├── business/
     │                   ├── infra/
     │                   │    ├── entity/
     │                   │    └── repository/
     └── resources/
          ├── application.properties
```

---

## 🛠️ Configurações e Perfis

- O projeto utiliza o perfil `dev` por padrão.
- Para alterar o perfil, edite o arquivo `application.properties`:
  ```
  spring.profiles.active=dev
  ```

---

## ☁️ Ambiente de Produção

- Recomenda-se configurar variáveis de ambiente para as credenciais sensíveis.
- Utilize um banco PostgreSQL gerenciado e configure HTTPS.

---

## 🤝 Contribuição

Contribuições são bem-vindas! Siga os passos:

1. Fork este repositório
2. Crie uma branch: `git checkout -b feature/sua-feature`
3. Commit suas alterações: `git commit -m 'feat: minha feature'`
4. Push na branch: `git push origin feature/sua-feature`
5. Abra um Pull Request

---