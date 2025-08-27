# Mood-Mirror



 Estrutura recomendada do projeto Spring Boot (API REST)


 
moodmirror-backend/
│
├── src/
│   ├── main/
│   │   ├── java/com/moodmirror/
│   │   │   ├── config/              # Configurações gerais (CORS, segurança, JWT, Swagger)
│   │   │   ├── controllers/         # Controllers (endpoints REST)
│   │   │   ├── dto/                 # DTOs (Data Transfer Objects)
│   │   │   ├── exceptions/          # Exceptions customizadas e handlers
│   │   │   ├── models/              # Entidades (JPA/Hibernate)
│   │   │   ├── repositories/        # Repositórios (Spring Data JPA)
│   │   │   ├── security/            # Configurações de autenticação/autorização
│   │   │   ├── services/            # Regras de negócio
│   │   │   ├── utils/               # Classes utilitárias (ex: conversores, validadores)
│   │   │   └── MoodMirrorApplication.java   # Classe principal
│   │   │
│   │   └── resources/
│   │       ├── application.yml      # Configurações (DB, JWT, etc.)
│   │       ├── logback-spring.xml   # Configuração de logs
│   │       └── messages.properties  # Mensagens de validação
│   │
│   └── test/java/com/moodmirror/    # Testes unitários e de integração
│
├── .gitignore
├── pom.xml (ou build.gradle)        # Dependências do projeto
└── README.md
