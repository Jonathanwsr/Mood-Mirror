# Moodmirror-backend
### Bem-vindo ao repositório do backend de MoodMirror, uma API REST desenvolvida com Spring Boot.
Modelos (Entidades Principais)

A seguir, as principais tabelas/entidades do sistema:

### User 
Representa o usuário da plataforma. Pode ter diferentes papéis (roles), como paciente, psicólogo ou administrador.

### UserRole 
Define os papéis de cada usuário no sistema, controlando permissões e acessos.

### Psychologist 
Contém dados de profissionais de psicologia, como especialização e número de licença.
Relaciona-se com User.

### Checkin 
Registro diário ou periódico do usuário sobre seu estado emocional. Pode conter texto ou mídia (imagem/áudio/vídeo).

### Analysis 
Resultado da análise feita pela IA sobre os checkins do usuário, identificando:

### Tendência de humor (mood trend)

### Resumo analítico

### Data da análise

### Recommendation 
Recomendações personalizadas geradas a partir das análises feitas pela IA.
Inclui dicas e categorias específicas para o usuário.

### TherapySession 
Sessões de terapia realizadas, vinculando paciente e psicólogo.

### Payment 
Controle de pagamentos das sessões ou serviços premium oferecidos na plataforma.

### UserMood 
Representa o humor do usuário em um determinado momento, utilizado pela IA para aprendizado e relatórios.
Este projeto foi estruturado para ser escalável e de fácil manutenção, seguindo as melhores práticas de arquitetura de software, com uma clara separação de responsabilidades em camadas.


# Tecnologias Utilizadas
Java 21


### Spring Boot 3.x

### Spring Security com JWT TOKEN

### Spring Data JPA

### Banco de Dados (aqui você pode escolher o banco, por exemplo: PostgreSQL, MySQL, H2)

JWT (JSON Web Tokens)

Swagger/OpenAPI (se estiver usando para documentação)

#  Como Executar o Projeto
Clone este repositório.

Configure as propriedades no arquivo src/main/resources/application.yml.

Execute a classe principal MoodMirrorApplication.java.


# Estrutura do Projeto
A seguir, a estrutura de diretórios do projeto, com uma breve descrição de cada componente:

```bash
moodmirror-backend/
├── src/
│   ├── main/
│   │   ├── java/com/moodmirror/
│   │   │   ├── config/             # Configurações gerais (CORS, segurança, JWT)
│   │   │   ├── controllers/        # Camada de apresentação (endpoints HTTP)
│   │   │   ├── dto/                # Objetos de transferência de dados
│   │   │   ├── exceptions/         # Exceções customizadas e handlers
│   │   │   ├── models/             # Entidades de domínio (JPA)
│   │   │   ├── repositories/       # Camada de acesso a dados (Spring Data JPA)
│   │   │   ├── security/           # Configurações de autenticação e autorização
│   │   │   ├── services/           # Regras de negócio
│   │   │   ├── utils/              # Classes utilitárias
│   │   │   └── MoodMirrorApplication.java
│   │   │
│   │   └── resources/
│   │       ├── application.yml     # Configurações do ambiente (DB, JWT etc.)
│   │       ├── logback-spring.xml  # Configurações de logging
│   │       └── messages.properties # Internacionalização e validações
│   │
│   └── test/java/com/moodmirror/   # Testes unitários e de integração
│
├── .gitignore                      # Arquivos ignorados pelo Git
├── pom.xml / build.gradle           # Gerenciador de dependências
└── README.md           


