# ✅ Checklist de Teste Smoke e Regressão

Este documento reúne exemplos de **checklist de Teste Smoke** e **Teste de Regressão**, aplicáveis a sistemas web como PDV, ERP ou aplicações de negócio.

---

## 🔥 Teste Smoke

### 🎯 Objetivo
Validar rapidamente se o sistema está **estável e testável** após um deploy, nova versão ou alteração significativa.

> ❌ Smoke falhou → testes devem ser bloqueados  
> ✅ Smoke passou → testes podem continuar

---

### 📋 Checklist de Smoke

- [ ] Sistema abre sem erros
- [ ] Login com usuário válido funciona
- [ ] Tela principal carrega corretamente
- [ ] Navegação entre menus funciona
- [ ] Funcionalidade principal do sistema abre (ex: Venda, Pedido, Cadastro)

---

### 🚨 Bloqueios comuns identificados no Smoke
- [ ] Tela branca ao acessar o sistema
- [ ] Erro crítico (ex: erro 500)
- [ ] Botões principais não respondem
- [ ] Falha de carregamento ou timeout

---

## 🔁 Teste de Regressão

### 🎯 Objetivo
Garantir que **funcionalidades já existentes continuam funcionando corretamente** após alterações no sistema, como correção de bugs ou implementação de novas funcionalidades.

---

### 🔐 Acesso
- [ ] Login com credenciais válidas
- [ ] Login com credenciais inválidas
- [ ] Logout funciona corretamente

---

### 🧾 Fluxo Principal do Sistema
- [ ] Criar novo processo (ex: nova venda)
- [ ] Inserir dados obrigatórios
- [ ] Inserir item ou produto
- [ ] Avançar no fluxo sem erros
- [ ] Finalizar processo com sucesso

---

### 💳 Regras de Negócio
- [ ] Aplicar desconto (quando aplicável)
- [ ] Validar formas de pagamento
- [ ] Bloqueios funcionam corretamente (ex: venda sem produto ou cliente)

---

### 🔄 Funcionalidades Relacionadas
- [ ] Editar registro existente
- [ ] Cancelar processo
- [ ] Reabrir processo
- [ ] Excluir registro (se aplicável)

---

### 🧭 Navegação
- [ ] Voltar entre telas sem perda de dados
- [ ] Cancelar ação no meio do fluxo
- [ ] Navegar entre menus sem comportamento inesperado

---

### 📄 Relatórios e Confirmações
- [ ] Gerar comprovante
- [ ] Visualizar histórico
- [ ] Exportar dados (quando disponível)

---

## ⚡ Checklist de Regressão (Versão Curta)
Utilizado quando o tempo para testes é reduzido.

- [ ] Login
- [ ] Fluxo principal completo
- [ ] Funcionalidade alterada
- [ ] Funcionalidades relacionadas
- [ ] Finalização sem erro

---

## 🧠 Observações
- O checklist de **Smoke** tende a ser fixo por sistema  
- O checklist de **Regressão** deve ser adaptado conforme a versão e as mudanças realizadas  
- Estes checklists podem ser utilizados em ferramentas como Jira, TestRail ou planilhas

---

📌 *Documento criado para fins de estudo e prática em QA.*
