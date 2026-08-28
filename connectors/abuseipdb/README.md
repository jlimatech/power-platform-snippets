# Conector Personalizado - AbuseIPDB

Conector personalizado (Custom Connector) para Power Automate que permite verificar **histórico de abuso**, **pontuação de reputação** e detalhes associados a um endereço IP usando o **AbuseIPDB**.

## 📌 Operações disponíveis

| Operação | Endpoint | Descrição |
|---|---|---|
| Obter informações sobre IP | `GET /check` | Retorna dados de reputação, reports e detalhes adicionais de um IP |

### Parâmetros

| Parâmetro | Tipo | Obrigatório | Descrição |
|---|---|---|---|
| `ipAddress` | string | Sim | Endereço IP a ser consultado |
| `maxAgeInDays` | integer | Não | Considera reports dos últimos N dias (padrão: 30) |
| `verbose` | boolean | Não | Retorna detalhes completos dos reports (padrão: false) |

## 🔑 Autenticação

O conector usa autenticação via **API Key**, enviada no header `Key`.

Você precisa de uma chave de API do AbuseIPDB, disponível em [abuseipdb.com](https://www.abuseipdb.com) (crie uma conta e acesse sua área de API).

## 🚀 Como importar no Power Automate

1. Acesse [make.powerautomate.com](https://make.powerautomate.com)
2. Vá em **Dados → Conectores personalizados**
3. Clique em **"Novo conector personalizado" → "Importar um arquivo OpenAPI"**
4. Faça upload do arquivo [`AbuseIP.swagger.json`](./AbuseIP.swagger.json)
5. Configure a segurança com sua API Key do AbuseIPDB
6. Teste e crie a conexão

## 📄 Arquivo

- [`AbuseIP.swagger.json`](./AbuseIP.swagger.json) - definição OpenAPI/Swagger 2.0 do conector
