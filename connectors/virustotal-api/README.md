# Conector Personalizado - VirusTotal API

Conector personalizado (Custom Connector) para Power Automate que permite consultar reputação de **IPs**, **domínios** e **arquivos (hash)** usando a API do VirusTotal.

## 📌 Operações disponíveis

| Operação | Endpoint | Descrição |
|---|---|---|
| Obter informações sobre IP | `GET /ip_addresses/{ip}` | Retorna reputação, localização e análises de um IP |
| Obter informações sobre domínio | `GET /domains/{domain}` | Retorna reputação, DNS, certificados e votos da comunidade |
| Obter informações sobre arquivo | `GET /files/{id}` | Retorna hashes, reputação e análises de um arquivo (MD5/SHA1/SHA256) |

## 🔑 Autenticação

O conector usa autenticação via **API Key**, enviada no header `x-apikey`.

Você precisa de uma chave de API do VirusTotal, disponível em [virustotal.com](https://www.virustotal.com) (crie uma conta e acesse seu perfil).

## 🚀 Como importar no Power Automate

1. Acesse [make.powerautomate.com](https://make.powerautomate.com)
2. Vá em **Dados → Conectores personalizados**
3. Clique em **"Novo conector personalizado" → "Importar um arquivo OpenAPI"**
4. Faça upload do arquivo [`VirusTotal-API-BCC.swagger.json`](./VirusTotal-API-BCC.swagger.json)
5. Configure a segurança com sua API Key do VirusTotal
6. Teste e crie a conexão

## 📄 Arquivo

- [`VirusTotal-API-BCC.swagger.json`](./VirusTotal-API-BCC.swagger.json) - definição OpenAPI/Swagger 2.0 do conector
