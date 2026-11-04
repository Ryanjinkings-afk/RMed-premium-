# RMed v12 — evolução da base funcional

## Alterações
- Reorganização da navegação com prioridade para Revalida, condutas, questões, casos e simulados.
- Página inicial redesenhada como central de preparação clínica.
- Nova trilha Revalida com grandes áreas, roteiro de estudo e atalhos para treino.
- Nova área Conta e interface de perfil local demonstrativo.
- Exportação local do progresso em JSON.
- Cache do service worker atualizado para v12.

## Limites importantes
A interface de perfil é apenas local/demonstrativa. Não é autenticação segura, não sincroniza dispositivos e não implementa assinaturas ou pagamentos. Não há armazenamento de senha. Para lançamento comercial, conectar Supabase Auth + banco PostgreSQL com políticas RLS, validação server-side de permissões e integração de pagamento via backend/webhook.

## Conteúdo clínico
O conteúdo clínico existente foi preservado. A nova trilha organiza o estudo, mas não significa que todos os tópicos listados já tenham uma aula ou banco de questões completo. As questões atuais são autorais e a base deve ser ampliada e revisada com referências oficiais antes de comercialização.

## Publicação
Substitua os arquivos do repositório pelo conteúdo desta pasta. Se o Safari mantiver a versão anterior, feche e reabra o site ou limpe os dados do site para renovar o cache.
