# 🔔 Aplicação de Notificações

Projeto full-stack com frontend em **HTML/CSS** e backend em **Java com Spring Boot**, para gerenciamento de notificações via API REST. Contém automação de testes e pipeline de CI/CD via GitHub Actions.

## Tecnologias utilizadas

- **Java 17** com **Spring Boot**
- Frontend em **HTML** e **CSS**
- **Spring Web** para API REST
- **Spring Data JPA** (com JDBC/Hibernate)
- **Banco de dados** configurável (MySQL, PostgreSQL, H2)
- **JUnit** e **Mockito** para testes unitários
- **Gradle** como build tool
- **GitHub Actions** para CI/CD

## Estrutura do Projeto

notificacao/
### ├── src/
### │ ├── main/
### │ │ ├── java/... # Código-fonte backend Java
### │ │ └── resources/
### │ │ └── static/ # Frontend HTML/CSS
### │ └── test/java/... # Testes unitários
### ├── build.gradle
### ├── settings.gradle
### ├── gradlew / gradlew.bat
### └── .github/workflows/ # Pipelines de CI/CD

## Como executar
1. Clonar o repositorio
  bash
  git clone https://github.com/alocss/notificacao.git
  cd notificacao

2. Build do projeto

  ./gradlew build

3. Executar localmente

  ./gradlew bootRun

A interface estática (HTML/CSS) pode ser acessada via localhost:8080 e os endpoints REST em /api/….

Configurações como porta e dados de conexão com banco podem ser ajustadas em application.properties ou .yml.
Testes automatizados

  ./gradlew test

Os testes estão localizados em src/test/java/, com cobertura de lógica e backend via JUnit 5 e Mockito.
Endpoints REST (exemplo)

Método	Endpoint	Descrição
### GET	/notifications	Lista notificações
### POST	/notifications	Cria nova notificação
### PUT	/notifications/{id}	Atualiza notificação existente
### DELETE	/notifications/{id}	Remove notificação

Verifique as classes de Controller para rotas exatas.
