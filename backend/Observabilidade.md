
**Observabilidade** é a capacidade de **entender o que está acontecendo dentro e um sistema** a partir dos dados que ele produz, **sem precisar alterar o código em produção**

### Os pilares da observabilidade são:

- **Logs**
- **Métricas**
- **Traces**

## Logs

Logs são **registros de eventos** que aconteceram na aplicação. Eles respondem a principal pergunta, **o que aconteceu ?**.

### Características

- São eventos pontuais
- Geralmente textuais ou em JSON
- Podem conter contexto (userId, requestId, erro, payload)
- Não seguem um intervalo fixo

### Exemplos de uso

- Erros e exceções
- Ações importantes do sistema
- Fluxos de negócio
- Debug em produção

```js
logger.info({ userId }, 'User created')
logger.warn({ email }, 'Login attempt failed')
logger.error(err, 'Unexpected error')
```

### Quando usar logs

- Investigar bugs
- Entender falhas específicas
- Auditar comportamentos

### Ferramentas comuns

- Pino
- Winston
- Bunyan
- ELK (Elastic + Logstash + Kibana)
- Grafana Loki
- Datadog Logs

## Métricas

### O que são

Métricas são valores numéricos agregados ao longo tempo. ***Elas respondem a pergunta:*** ***Como o sistema está se comportando***.

### Exemplos de métricas

- Latência média das requisições 
- Número de requisições por segundo (RPS)
- Uso de CPU e memória
- Taxa de erro (%)
- Número de usuários ativos

### Exemplo

```txt
http_requests_total = 10239
http_request_duration_ms_avg = 120
cpu_usage_percent = 68

```

### Quando usar métricas

- Monitoramento em tempo real
- Alertas (ex: CPU > 80%)
- Análise de performance
- Capacidade e escalabilidade

### Ferramentas comuns

- Prometheus
- Grafana
- OpenTelemetry
- Datadog Metrics
- New Relic

## Traces

### O que são

Traces representaram  ***o caminho completo de uma requisição*** passando por um ou vários serviços. Eles respondem à pergunta: ***Por onde essa requisição passou e quanto tempo levou em cada etapa?***

### Conceitos importantes

- **Trace** → fluxo completo de uma requisição
- **Span** → um passo dentro do trace    
- **Trace ID** → identificador único do fluxo
- **Span ID** → identificador de cada operação

### Exemplo de trace

```mathematica
Trace ID: abc123
├── HTTP Request (API) – 120ms
│   ├── Auth Service – 30ms
│   ├── Database Query – 70ms
│   └── Cache – 10ms
```

### Quando usar traces

- Identificar gargalos de performance
- Entender latência em microsserviços
- Debug de requisições lentas
- Correlacionar logs com uma requisição específica

### Ferramentas comuns

- OpenTelemetry
- Jaeger
- Zipkin
- Datadog APM
- New Relic APM


## 🔗 Relação entre Logs, Métricas e Traces

Eles **se complementam**, não se substituem.

| Pilar    | Pergunta principal       |
| -------- | ------------------------ |
| Logs     | O que aconteceu?         |
| Métricas | O sistema está saudável? |
| Traces   | Onde está o gargalo?     |

### Exemplo prático

- 📈 Métrica mostra aumento de latência
- 🧵 Trace identifica a query lenta
- 🪵 Log mostra o erro ou contexto exato