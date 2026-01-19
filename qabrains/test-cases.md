# 📋 Casos de Teste – QA Brains

| ID | Cenário | Passos | Resultado Esperado | Status |
|----|----------|--------|--------------------|--------|
| CT-QAB01 | Login válido | 1. Acessar https://practice.qabrains.com/2. Inserir e-mail `qa_testers@qabrains.com`<br>3. Inserir senha `Password123`<br>4. Clicar em “Login” | Mensagem "Login Successful" é exibida ao usuário | ✅ |
| CT-QAB02 | Login inválido | 1. Inserir e-mail `qa_testers@qabrains.com`<br>2. Inserir senha incorreta<br>3. Clicar em “Login” | Mensagem “Your password is invalid!” é exibida | ✅ |
| CT-QAB03 | Reset com e-mail válido | 1. Clicar em "Forgot Password"<br>2. Inserir e-mail `qa_testers@qabrains.com`<br>3. Clicar em "Reset Password" | Mensagem "Password is reset successfully." | ✅ |
| CT-QAB04 | Reset com e-mail inválido | 1. Clicar em "Forgot Password"<br>2. Inserir e-mail `qa_testers`<br>3. Clicar em "Reset Password" | Mensagem "Inclua um "@" no endereço de e-mail. "qa_testers" esta com um "@" faltando." | ✅ |

Legenda:  
✅ = Passou 🟡 = Falhou ❌ = Bloqueado 🔄 = Retestar
