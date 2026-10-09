# E-tiquete

Plataforma de venda e reserva de ingressos desenvolvida com arquitetura de microsserviços, com foco em confiabilidade, desempenho e consistência em cenários de alta concorrência.

## Sobre o projeto

O Etiquete busca evitar problemas comuns em vendas de ingressos de alta demanda, como venda duplicada de assentos, cobranças em duplicidade e reservas abandonadas.

A plataforma permitirá consultar eventos, reservar assentos temporariamente, realizar pagamentos simulados e receber confirmações. Em caso de falha no pagamento ou expiração da reserva, o sistema deverá liberar o assento automaticamente.

## Arquitetura

O sistema prevê os seguintes serviços:

- API Gateway
- Catálogo de Eventos
- Reserva de Assentos
- Pedidos
- Pagamento
- Notificações

## Tecnologias

- NodeJS + React
- Postgres
- Redis
- Docker Composer
- GitHub Actions

*A stack definitiva será confirmada durante o desenvolvimento do projeto.*

## Padrões arquiteturais

- Saga com orquestração
- Transactional Outbox
- Retry e Dead Letter Queue (DLQ)
- Circuit Breaker
- Cache-Aside
- Database per Service
- API Gateway

## Objetivos

- Evitar a venda duplicada de assentos.
- Garantir a idempotência das operações de pagamento.
- Liberar reservas expiradas automaticamente.
- Manter a disponibilidade dos serviços diante de falhas.
- Monitorar o desempenho sob alta concorrência.
- Garantir a entrega confiável de eventos entre os serviços.

## Status

Em desenvolvimento.

