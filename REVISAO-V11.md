# RMed v11 — expansão das ferramentas clínicas

## Alterações nesta versão
- Preservada a base monolítica funcional do RMed v10, com identidade visual, navegação, português/espanhol, farmacologia, antimicrobianos, protocolos, consulta clínica, questões, simulados, casos, flashcards e progresso local.
- Adicionada calculadora de dose por peso: permite converter uma dose de referência em mg/kg/dose ou mg/kg/dia para mg por administração e mL por administração, com frequência, concentração disponível e limite máximo opcional informado pelo usuário.
- Adicionada calculadora de balanço hídrico de 24 horas, na sequência PI, DD, DH, LI, LE e BH, usando os fatores de perdas insensíveis configurados (homem 0,5; mulher 0,6).
- Adicionadas traduções espanholas para os novos campos e avisos.
- Atualizada a versão do service worker/cache para v11 para reduzir risco de servir a interface antiga após publicação.

## Segurança e limites
- A calculadora de dose não escolhe medicamento, indicação ou dose terapêutica; apenas converte matematicamente os valores fornecidos. Conferir prescrição, faixa etária, dose máxima, concentração e protocolo vigente.
- O balanço hídrico usa a fórmula educacional indicada no projeto. Perdas insensíveis são estimativas e podem variar muito conforme contexto clínico.
- Não foram adicionados login, sincronização em nuvem, pagamentos ou assinatura nesta etapa.
- Conteúdo e cálculos exigem revisão clínica independente antes de uso assistencial. O RMed é material educacional e não substitui protocolos institucionais nem julgamento profissional.
