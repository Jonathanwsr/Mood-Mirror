# Moodmirror-backend
### Bem-vindo ao repositório do backend de MoodMirror, uma API REST desenvolvida com Spring Boot.

Este projeto foi estruturado para ser escalável e de fácil manutenção, seguindo as melhores práticas de arquitetura de software, com uma clara separação de responsabilidades em camadas.

# Estrutura do Projeto
A seguir, a estrutura de diretórios do projeto, com uma breve descrição de cada componente:

moodmirror-backend/
├── src/
│   ├── main/
│   │   ├── java/com/moodmirror/
│   │   │   ├── config/             # Configurações gerais da aplicação (CORS, segurança, JWT).
│   │   │   ├── controllers/        # Camada de Apresentação. Recebe e processa as requisições HTTP.
│   │   │   ├── dto/                # Objetos de Transferência de Dados (DTOs).
│   │   │   ├── exceptions/         # Gerenciamento de exceções customizadas.
│   │   │   ├── models/             # Entidades de domínio mapeadas para o banco de dados (JPA).
│   │   │   ├── repositories/       # Camada de Acesso a Dados (Spring Data JPA).
│   │   │   ├── security/           # Configurações de segurança e autenticação (JWT).
│   │   │   ├── services/           # Camada de Negócio. Contém a lógica principal da aplicação.
│   │   │   ├── utils/              # Classes utilitárias com funcionalidades genéricas.
│   │   │   └── MoodMirrorApplication.java
│   │   │
│   │   └── resources/
│   │       ├── application.yml     # Configurações de ambiente (banco de dados, JWT).
│   │       ├── logback-spring.xml  # Configurações de logging.
│   │       └── messages.properties # Mensagens para internacionalização e validações.
│   │
│   └── test/java/com/moodmirror/   # Código para testes unitários e de integração.
│
├── .gitignore                      # Define quais arquivos e diretórios o Git deve ignorar.
├── pom.xml (ou build.gradle)       # Gerenciador de dependências.
└── README.md                       # Este arquivo.

Tecnologias Utilizadas
Java 21

Spring Boot 3.x

Spring Security

Spring Data JPA

Banco de Dados (aqui você pode especificar o banco, por exemplo: PostgreSQL, MySQL, H2)

JWT (JSON Web Tokens)

Swagger/OpenAPI (se estiver usando para documentação)

#  Como Executar o Projeto
Clone este repositório.

Configure as propriedades no arquivo src/main/resources/application.yml.

Execute a classe principal MoodMirrorApplication.java.

