# Implementacao-de-Proxies---Insurance-Policy-Management-System

**README - Implementação de Proxies em Python**

Este é um breve guia sobre  os proxies  implementados no código. O código apresenta o uso de proxies para controle de acesso e segurança em torno das operações realizadas em instâncias das classes `Customer` e `Policy`.

### Introdução aos Proxies

Os proxies são padrões de design que atuam como intermediários entre um cliente e um objeto real. Eles controlam o acesso ao objeto real, adicionando uma camada de abstração e segurança. No código fornecido, dois tipos de proxies são implementados: `CustomerProxy` e `PolicyProxy`.

### Implementação dos Proxies

- **`CustomerProxy`**: Este proxy é usado para controlar o acesso às informações do cliente e às operações relacionadas a políticas associadas a esse cliente. Ele contém métodos como `view_personal_info()` para visualizar informações pessoais do cliente e `add_policy()` para adicionar uma nova apólice ao perfil do cliente.

- **`PolicyProxy`**: Este proxy é responsável por controlar o acesso aos detalhes da política e às operações relacionadas ao processamento de pagamentos e reivindicações. Ele contém métodos como `view_policy_details()` para visualizar os detalhes da apólice e `process_payment()` para processar pagamentos.

### Uso dos Proxies

No código , os proxies são utilizados principalmente dentro da função `user_interface()`. Um exemplo de uso é quando um cliente tenta adicionar uma apólice ao seu perfil. Em vez de adicionar diretamente a apólice ao perfil do cliente, o proxy `CustomerProxy` é usado para adicionar a apólice. Isso permite que o proxy execute verificações de segurança ou autorização antes de permitir a adição da apólice ao perfil do cliente.

### Conclusão

Os proxies são uma ferramenta poderosa para controlar o acesso a objetos e operações sensíveis em uma aplicação. Eles fornecem uma maneira elegante de adicionar camadas de segurança e abstração, garantindo que as operações sejam executadas de maneira segura e controlada. No código fornecido, os proxies `CustomerProxy` e `PolicyProxy` desempenham um papel fundamental na garantia da segurança e controle de acesso às informações do cliente e detalhes da política.
