# Português (pt-br)

## Passos para Configuração do SigNoz

### Adicionar o repositório Helm do SigNoz

```sh
helm repo add signoz https://charts.signoz.io
kubectl create ns platform
helm --namespace platform install signoz signoz/signoz -f values.yaml
```

## Configuração do service

```sh
kubectl edit svc -n platform signoz-otel-collector
```

## Configuração do ingress

```sh
kubectl edit ingres -n platform signoz-frontend
```

# English

## Steps to Setup SigNoz

### Add the SigNoz Helm repository

```sh
helm repo add signoz https://charts.signoz.io
kubectl create ns platform
helm --namespace platform install signoz signoz/signoz -f values.yaml
```

## Service setup

```sh
kubectl edit svc -n platform signoz-otel-collector
```

## Ingress setup

```sh
kubectl edit ingres -n platform signoz-frontend
```
