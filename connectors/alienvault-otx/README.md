# Conector Personalizado - AlienVault OTX

Conector personalizado (Custom Connector) para Power Automate que permite consultar informações de reputação e threat intelligence de endereços **IPv4** usando o **AlienVault OTX** (Open Threat Exchange).

## 📌 Operações disponíveis

| Operação | Endpoint | Descrição |
|---|---|---|
| Obter informações de IPv4 | `GET /v1/indicators/IPv4/{IP}/general` | Retorna informações gerais sobre um endereço IPv4 (indicadores, pulses, reputação) |

## 🔑 Autenticação

O conector usa autenticação via **API Key**, enviada no header `X-OTX-API-KEY`.

Você precisa de uma chave de API do AlienVault OTX, disponível em [otx.alienvault.com](https://otx.alienvault.com) (crie uma conta gratuita e acesse suas configurações de API).

## 🚀 Como importar no Power Automate

1. Acesse [make.powerautomate.com](https://make.powerautomate.com)
2. Vá em **Dados → Conectores personalizados**
3. Clique em **"Novo conector personalizado" → "Importar um arquivo OpenAPI"**
4. Faça upload do arquivo [`ALIEN-VAULT-OTX.swagger.json`](./ALIEN-VAULT-OTX.swagger.json)
5. Configure a segurança com sua API Key do AlienVault OTX
6. Teste e crie a conexão

## 📄 Arquivo

- [`ALIEN-VAULT-OTX.swagger.json`](./ALIEN-VAULT-OTX.swagger.json) - definição OpenAPI/Swagger 2.0 do conector
