# Auditoria técnica RMed v11

- Base v10 preservada e modificada diretamente; não houve reconstrução da aplicação.
- JavaScript inline extraído para `inline-check.js` e validado com `node --check`.
- IDs HTML verificados: 111 IDs, sem duplicatas.
- Service worker atualizado para cache v11 e registro `sw.js?v=11.0`.
- Novos cálculos adicionados: conversão de dose por peso e balanço hídrico de 24 horas.
- Ainda não foi realizado teste visual em Safari/iPhone nem validação clínica independente. A publicação no GitHub Pages deve ser conferida após o upload.
