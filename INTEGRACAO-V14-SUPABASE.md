# RMed Premium V14 — autenticação Supabase

## O que foi alterado
- Substituído o perfil local demonstrativo por autenticação real do Supabase.
- Cadastro com nome, e-mail e senha.
- Login com e-mail e senha.
- Confirmação de cadastro por e-mail (conforme configuração do projeto Supabase).
- Recuperação de senha por e-mail e formulário de definição de nova senha.
- Exibição do estado da conta e do plano Free/Premium consultado na tabela `profiles`.
- Mantido o progresso de estudo local no navegador; a sincronização do progresso não faz parte desta etapa.
- Atualizado o cache do service worker para a versão V14.

## Configuração usada
- Project URL: `https://hkmoqzpvxthfhyoavddd.supabase.co`
- Publishable key: chave `sb_publishable_` fornecida pelo proprietário.
- A chave publicável é destinada ao frontend. Nenhuma `sb_secret_` ou `service_role` foi incluída.

## Publicação
1. Faça backup da versão atual do repositório Premium.
2. Extraia o conteúdo desta pasta.
3. Envie todos os arquivos da pasta `RMed_Premium` para a raiz do repositório `RMed-premium-`, substituindo os arquivos correspondentes.
4. Aguarde o GitHub Pages concluir a publicação.
5. Abra o site em uma janela privada ou limpe o cache do site para evitar o service worker antigo.

## Testes após publicar
1. Abra o site e vá a Entrar / Criar conta.
2. Crie uma conta de teste com um e-mail acessível e senha de pelo menos 8 caracteres.
3. Confirme o e-mail recebido.
4. Volte ao site e faça login.
5. Em Supabase > Authentication > Users, confirme a existência do usuário.
6. Em Table Editor > `profiles`, confirme o perfil criado automaticamente.

## Limites desta versão
- O pagamento do Mercado Pago ainda NÃO libera Premium automaticamente.
- A integração de cobrança precisa de uma Edge Function/backend que crie ou consulte a assinatura e valide notificações/webhooks do Mercado Pago.
- A tabela `profiles` só permite leitura do próprio perfil pelo usuário; a atualização de plano deve ser feita exclusivamente por função confiável no servidor.
- O progresso ainda permanece no armazenamento local do navegador.
- A chave publicável pode ficar no frontend; nunca publicar chaves secretas, service role, access tokens ou credenciais do Mercado Pago.

## Importante
Não use a interface do navegador para editar manualmente `plan='premium'`. A liberação será implementada somente após a validação do pagamento no servidor.
