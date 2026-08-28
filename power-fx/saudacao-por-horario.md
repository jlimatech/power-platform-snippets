# Saudação por Horário

Retorna uma saudação em português ("Bom dia!", "Boa tarde!" ou "Boa noite!") com base no horário atual, considerando o fuso horário de Brasília (E. South America Standard Time).

## Lógica

- **05h–12h** → "Bom dia!"
- **12h–18h** → "Boa tarde!"
- **Fora desse intervalo** → "Boa noite!"

## Código

```powerfx
if(
  and(
    greaterOrEquals(int(formatDateTime(convertTimeZone(utcNow(),'UTC','E. South America Standard Time'),'HH')),5),
    less(int(formatDateTime(convertTimeZone(utcNow(),'UTC','E. South America Standard Time'),'HH')),12)
  ),
  'Bom dia!',
  if(
    and(
      greaterOrEquals(int(formatDateTime(convertTimeZone(utcNow(),'UTC','E. South America Standard Time'),'HH')),12),
      less(int(formatDateTime(convertTimeZone(utcNow(),'UTC','E. South America Standard Time'),'HH')),18)
    ),
    'Boa tarde!',
    'Boa noite!'
  )
)
```

## Uso

Cole essa expressão em um campo de texto dinâmico (ex: corpo de e-mail, mensagem de Teams/Adaptive Card) dentro de um fluxo do Power Automate.

## Observações

- O fuso horário `E. South America Standard Time` corresponde ao horário de Brasília (UTC-3).
- Para outro fuso, troque o nome do fuso na função `convertTimeZone`.
