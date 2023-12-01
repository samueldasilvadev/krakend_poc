# krakend poc
...

## DoD
- Configurações
- Autenticação
    - Gateway
    - Microsservices
- Erros
    - Logs
    - Tratamento de Erros
    - ChatOps
- Segurança
- Escala
- Observabilidade
    - Integração com ferramentas de telemetria
    - Monitoramento a nível de infra
    - Monitoramento a nível de serviço
- Deploy
- Comparativo com outras soluções

## Headers
X-Krakend-Completed: true se retornar os dados de todas as requisições, false se uma falhar

## Build plugin
```bash
docker run -it -v "$PWD:/app" -w /app \
krakend/builder:2.5.0 \
go build -buildmode=plugin -o krakend-server-example.so .
```
