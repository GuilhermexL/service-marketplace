# Local Services Marketplace

Bem-vindo ao repositório do **Local Services Marketplace**, uma plataforma projetada para conectar prestadores de serviços locais com clientes em busca de soluções rápidas e confiáveis. Este projeto foi desenvolvido utilizando **Java** e tecnologias como **Spring Boot**, **JPA** e **JDBC**.

---

## Funcionalidades Principais
- **Registro de Usuários**: Cadastro de prestadores e clientes.
- **Listagem de Serviços**: Consulta de serviços locais disponíveis.
- **Busca Avançada**: Filtragem por categoria, preço e localização.
- **Agendamento de Serviços**: Solicitação e gerenciamento de agendamentos.
- **Sistema de Avaliações**: Clientes podem avaliar e comentar serviços prestados.

---

## Tecnologias Utilizadas
- **Linguagem**: Java 17
- **Framework**: Spring Boot
- **Banco de Dados**: H2 para desenvolvimento e PostgreSQL para produção
- **Persistência de Dados**: JPA (Hibernate) e JDBC
- **Segurança**: Spring Security com autenticação JWT
- **Testes**: JUnit e Mockito
- **Ferramentas Auxiliares**: Lombok, ModelMapper e Flyway

---

## Autores

- Guilherme Santos: https://github.com/GuilhermexL
- Mateus Tomaz: https://github.com/mateustomaz1
- Klebson Amarante: https://github.com/KlebsonAmaranteS
---

## Como Executar o Projeto

### 1. Requisitos
- Java 17 ou superior
- Maven 3.8+
- PostgreSQL (opcional para produção)

### 2. Passos
1. Clone o repositório:
   ```bash
   git clone https://github.com/GuilhermexL/service-marktplace.git
   ```
2. Navegue até a pasta do projeto:
   ```bash
   cd local-services-marketplace
   ```
3. Configure o arquivo `application.yml` em `src/main/resources` para o ambiente desejado.
4. Execute o seguinte comando para rodar o projeto:
   ```bash
   mvn spring-boot:run
   ```
5. O projeto estará acessível em: [http://localhost:8080](http://localhost:8080)

---

## Rotas Principais da API

### Autenticação
- `POST /auth/register` - Registro de novo usuário
- `POST /auth/login` - Login e geração de token JWT

### Serviços
- `GET /services` - Listar todos os serviços
- `POST /services` - Criar um novo serviço (restrito a prestadores)
- `GET /services/{id}` - Detalhes de um serviço específico

### Agendamentos
- `POST /appointments` - Criar um novo agendamento
- `GET /appointments` - Listar agendamentos do usuário logado

### Avaliações
- `POST /reviews` - Avaliar um serviço
- `GET /reviews/{serviceId}` - Consultar avaliações de um serviço

---

## Contribuição
Contribuições são bem-vindas! Siga os passos abaixo:
1. Realize um fork deste repositório.
2. Crie uma nova branch:
   ```bash
   git checkout -b minha-feature
   ```
3. Implemente suas alterações e faça commits:
   ```bash
   git commit -m "Adiciona nova funcionalidade X"
   ```
4. Envie as alterações para o seu fork:
   ```bash
   git push origin minha-feature
   ```
5. Abra um Pull Request neste repositório.

---

## Licença
Este projeto está licenciado sob a [MIT License](LICENSE).
