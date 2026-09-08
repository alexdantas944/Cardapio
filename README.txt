SONHO DE PASTEL — CHECKOUT V2

1. Abra index.html.
2. Configure:
   SUPABASE_URL
   SUPABASE_ANON_KEY
   WHATSAPP
   DELIVERY_FEE
3. No Supabase, execute supabase_schema.sql.
4. Crie o bucket público "produtos".
5. Cadastre os produtos na tabela produtos e coloque o caminho da foto no campo imagem.
6. O cliente:
   Cardápio -> Carrinho -> Dados -> Revisão -> WhatsApp.
7. Antes de abrir o WhatsApp, o checkout tenta salvar o pedido na tabela pedidos.
8. Se o Supabase estiver indisponível, o WhatsApp continua funcionando e gera um código local de pedido.

IMPORTANTE:
- Use somente a chave ANON pública no navegador.
- Nunca coloque a service_role key no HTML.
- A política pública de INSERT em pedidos é intencional para o checkout; não permita SELECT/UPDATE/DELETE público.
