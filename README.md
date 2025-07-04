
```markdown
# Cadastro de Usuário

Este projeto é uma aplicação backend que expõe uma API RESTful para gerenciamento de usuários. 
O sistema foi construído com foco em boas práticas de desenvolvimento, como separação de camadas (controller, service, repository).

---

## 🚀 Tecnologias Utilizadas

- Java 17
- Spring Boot 3.x: Spring Web e Spring Data JPA
- Maven 3.8+
- Banco de Dados: H2
- Lombok

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
## 📜 Endpoints Disponíveis
| Método | Endpoint      | Descrição                            |
|--------|---------------|--------------------------------------|
| GET    | /usuarios     | Lista todos os usuários              |
| POST   | /usuarios     | Cria um novo usuário                 |
| PUT    | /usuarios     | Atualiza um usuário pelo ID e e-mail |
| DELETE | /usuarios     | Deleta um usuário pelo e-mail        |

## 🤝 Contribuição

Contribuições são bem-vindas! Siga os passos:

1. Fork este repositório
2. Crie uma branch: `git checkout -b feature/sua-feature`
3. Commit suas alterações: `git commit -m 'feat: minha feature'`
4. Push na branch: `git push origin feature/sua-feature`
5. Abra um Pull Request

---