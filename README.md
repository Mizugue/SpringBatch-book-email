📚 Spring Batch - Book Email Notification

Este projeto é uma aplicação Spring Boot que utiliza Spring Batch para enviar notificações por e-mail a usuários que possuem empréstimos de livros próximos da data de devolução.
🚀 Funcionalidades

    📖 Leitura de usuários com livros cujo prazo de devolução está próximo.

    🛠 Processamento das informações para gerar mensagens personalizadas.

    📩 Envio automático de e-mails de notificação.

    🗄 Persistência com Spring Data JPA.

    🗃 Inicialização de dados com import.sql.

🛠 Tecnologias Utilizadas

    Java 17+

    Spring Boot

    Spring Batch

    Spring Data JPA

    Maven

    H2 Database (padrão, pode ser alterado)

    Jakarta Mail / JavaMailSender


🔄 Fluxo do Batch

flowchart TD
    A[Start Job] --> B[Read Users with Loans Close to Return]
    B --> C[Process Loan Data - Format Email Content]
    C --> D[Send Email Notification]
    D --> E[Job Finished]
