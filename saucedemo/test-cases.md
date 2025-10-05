# 📋 Casos de Teste – SauceDemo

| ID | Cenário | Passos | Resultado Esperado | Status |
|----|----------|--------|--------------------|--------|
| CT01 | Login válido | 1. Acessar https://www.saucedemo.com/<br>2. Inserir usuário `standard_user`<br>3. Inserir senha `secret_sauce`<br>4. Clicar em “Login” | Usuário é redirecionado à página de produtos | ✅ |
| CT02 | Login inválido | 1. Inserir usuário `standard_user`<br>2. Inserir senha incorreta<br>3. Clicar em “Login” | Mensagem “Username and password do not match” é exibida | ✅ |
| CT03 | Adicionar produto ao carrinho | 1. Fazer login válido<br>2. Clicar em “Add to cart” no primeiro produto<br>3. Acessar o ícone do carrinho | Produto aparece listado no carrinho | ✅ |
| CT04 | Remover produto do carrinho | 1. Adicionar um produto<br>2. Acessar o carrinho<br>3. Clicar em “Remove” | Produto é removido da lista | ✅ |
| CT05 | Finalizar compra com sucesso | 1. Adicionar produto<br>2. Acessar carrinho<br>3. Clicar em “Checkout”<br>4. Preencher os dados e concluir | Mensagem “Thank you for your order!” é exibida | ✅ |
| CT06 | Finalizar compra sem produtos | 1. Ir ao carrinho vazio<br>2. Clicar em “Checkout” | Mensagem “Cart is empty” deve ser exibida | 🟡 (Falhou) |

Legenda:  
✅ = Passou 🟡 = Falhou ❌ = Bloqueado 🔄 = Retestar
