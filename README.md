# SMTP Utilities Microservice

## Descrição
Este projeto consiste em um conjunto de microsserviços para facilitar o envio e gerenciamento de e-mails através do protocolo SMTP. Utilizamos a arquitetura clean para manter a organização e escalabilidade do código, Kafka para comunicação entre os serviços e Docker para conteinerização e fácil implantação.

## Funcionalidades

- **Envio de E-mails**: Suporte a envios simples, múltiplos e com anexos.
- **Autenticação SMTP**: Suporta servidores que exigem autenticação.
- **Configuração Dinâmica**: Permite configuração dos servidores SMTP pelos usuários.
- **Templates de E-mail**: Utilização de templates para envios personalizados.
- **Agendamento de E-mails**: Permite agendar o envio de e-mails.
- **Logs de E-mails**: Registra tentativas de envio, incluindo erros e sucessos.
- **Validação de E-mail**: Verifica a validade dos endereços de e-mail.
- **Rate Limiting**: Limita a quantidade de e-mails enviados num intervalo de tempo.
- **Fila de Envio**: Gerenciamento de fila de e-mails para lidar com alto volume.
- **Relatórios e Estatísticas**: Geração de relatórios sobre as atividades de e-mail.
- **API de Integração**: Facilita a integração com outras aplicações.
- **Monitoramento e Alertas**: Monitora o serviço e alerta sobre falhas.

## Arquitetura

### Microsserviços
O projeto é dividido em microsserviços, cada um responsável por uma parte específica do processo de e-mail. A comunicação entre eles é feita através do Apache Kafka, garantindo desacoplamento e resiliência.

### Clean Architecture
Adotamos a Clean Architecture para promover a separação de interesses dentro de cada serviço. Isso facilita a manutenção e a escalabilidade do código.

## Tecnologias Utilizadas

- **Apache Kafka**: Para comunicação assíncrona entre os serviços.
- **Docker**: Para conteinerização e implantação dos serviços.
- **Linguagem de Programação**: .NET 9.0

## Configuração e Execução

### Pré-requisitos
- Docker
- Docker Compose
- Apache Kafka (pode ser configurado e executado via Docker)

### Instalação
1. Clone o repositório:
    git clone [URL-do-repositório]
2. Utilize Docker Compose para construir e executar os serviços:
    docker-compose up --build


## Licença

Este projeto está licenciado sob a Licença MIT - veja o arquivo [LICENSE.md](LICENSE.md) para detalhes.