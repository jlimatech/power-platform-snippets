# Power Platform Snippets

![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)
![Power Platform](https://img.shields.io/badge/Microsoft-Power%20Platform-742774?logo=microsoft)

Coleção de snippets úteis para **Power Automate**, **Power Fx** e **Conectores Personalizados** - expressões, fórmulas, fluxos e definições de API prontas para copiar, adaptar e aplicar em seus ambientes.

## 🚀 Como Usar

### Power Fx / Power Automate
Navegue até a categoria desejada, abra o arquivo do snippet, copie a expressão ou fórmula e adapte as variáveis de acordo com as necessidades do seu projeto.

### Conectores Personalizados (Custom Connectors)
Para utilizar os conectores personalizados:
1. Navegue até a pasta do conector desejado em `./connectors/NOME_DO_CONECTOR/`.
2. Baixe o arquivo de definição OpenAPI (`.json` ou `.yaml`).
3. Acesse o [Power Automate](https://make.powerautomate.com) ou [Power Apps](https://make.powerapps.com).
4. Vá em **Dados** > **Conectores Personalizados** > **Novo conector personalizado** > **Importar um arquivo OpenAPI**.
5. Configure as chaves de API / autenticação necessárias e salve o conector.

## 📂 Estrutura do Repositório

- [`power-fx/`](./power-fx) - Expressões, fórmulas e lógicas reutilizáveis em Power Fx
- [`power-automate/`](./power-automate) - Fluxos, lógicas e expressões avançadas para Power Automate
- [`connectors/`](./connectors) - Conectores personalizados (Custom Connectors) em formato OpenAPI / Swagger

## 📋 Índice de Snippets

| Snippet | Categoria | Descrição |
|---|---|---|
| [Saudação por horário](./power-fx/saudacao-por-horario.md) | Power Fx | Retorna "Bom dia!", "Boa tarde!" ou "Boa noite!" com base no horário atual (fuso E. South America). |
| [VirusTotal API](./connectors/virustotal-api/) | Conector Personalizado | Consulta reputação de IPs, domínios e hashes de arquivos via VirusTotal. |
| [AlienVault OTX](./connectors/alienvault-otx/) | Conector Personalizado | Consulta threat intelligence e indicadores de comprometimento de IPs via AlienVault OTX. |
| [AbuseIPDB](./connectors/abuseipdb/) | Conector Personalizado | Verifica histórico de abuso, pontuação de confiança e reputação de IPs via AbuseIPDB. |

## 🤝 Contribuindo

Contribuições são sempre bem-vindas! Sinta-se à vontade para abrir uma **Issue** ou enviar um **Pull Request** sugerindo novos snippets, melhorias em fluxos existentes ou novos conectores personalizados.

## 📄 Licença

Este projeto está sob a licença MIT - veja o arquivo [LICENSE](./LICENSE) para mais detalhes.
| [AlienVault OTX](./connectors/alienvault-otx/) | Conector Personalizado | Consulta threat intelligence de endereços IPv4 via AlienVault OTX |
| [AbuseIPDB](./connectors/abuseipdb/) | Conector Personalizado | Verifica histórico de abuso e reputação de IPs via AbuseIPDB |

## 🤝 Contribuindo

Sinta-se à vontade para abrir uma issue ou PR sugerindo novos snippets, fluxos ou conectores.

## 📄 Licença

Este projeto está sob a licença MIT - veja o arquivo [LICENSE](./LICENSE) para mais detalhes.
