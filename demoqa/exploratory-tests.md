# 🧠 Testes Exploratórios e de Usabilidade – DemoQA

## 1. Introdução
O site **[DemoQA](https://demoqa.com/)** oferece diversos componentes interativos (botões, formulários, alerts, tabelas etc.) voltados para práticas de automação e teste manual.

O objetivo deste documento é registrar observações e resultados obtidos durante a execução de **testes exploratórios e de usabilidade**, com foco em identificar inconsistências, falhas de interface e comportamentos inesperados.

---

## 2. Abordagem de Teste
- Tipo: Teste exploratório e de usabilidade  
- Áreas avaliadas:  
  - Formulários (“Forms”)  
  - Botões (“Buttons”)  
  - Alertas e pop-ups (“Alerts, Frame & Windows”)  
  - Tabelas (“Web Tables”)  

---

## 3. Heurísticas de Usabilidade Consideradas
| Heurística | Descrição | Observação |
|-------------|------------|-------------|
| Visibilidade do status do sistema | O usuário deve saber o que está acontecendo | Algumas ações não exibem feedback imediato |
| Consistência e padrões | Elementos devem seguir o mesmo padrão visual | Pequenas variações de tamanho em botões |
| Prevenção de erros | A interface deve evitar erros do usuário | Campos aceitam valores inválidos sem aviso |
| Estética e design minimalista | A tela deve ser limpa e intuitiva | Alguns elementos estão sobrepostos em telas pequenas |

---

## 4. Cenários Testados

### Cenário 1 – Formulário de Cadastro
**Passos:**
1. Acessar [demoqa.com/forms](https://demoqa.com/forms)  
2. Preencher todos os campos obrigatórios  
3. Clicar em “Submit”  

**Resultado esperado:**  
Mensagem de sucesso “Form submitted successfully” exibida abaixo do botão.

**Resultado obtido:**  
✅ O formulário é enviado corretamente.  
📝 Observação: não há destaque visual indicando campos obrigatórios antes do envio (poderia ser melhorado).

---

### Cenário 2 – Botões de Ação
**Passos:**
1. Acessar [demoqa.com/buttons](https://demoqa.com/buttons)  
2. Clicar uma vez, duplo clique e clique com o botão direito  

**Resultado esperado:**  
Cada tipo de clique exibe a mensagem correspondente.  

**Resultado obtido:**  
✅ Funcionou corretamente em desktop.  

---

### Cenário 3 – Alertas e Pop-ups
**Passos:**
1. Acessar [demoqa.com/alerts](https://demoqa.com/alerts)  
2. Clicar nos botões “Click me” e “Timer Alert Button”  

**Resultado esperado:**  
Alertas devem ser exibidos conforme a ação.  

**Resultado obtido:**  
🟡 Em alguns casos o alerta não é exibido após o tempo configurado (Chrome).  

---

### Cenário 4 – Tabelas Interativas
**Passos:**
1. Acessar [demoqa.com/webtables](https://demoqa.com/webtables)  
2. Clicar em “Add” e inserir novos dados  
3. Testar edição e exclusão  

**Resultado esperado:**  
Tabela deve ser atualizada conforme as ações.  

**Resultado obtido:**  
✅ Edição e exclusão funcionam corretamente.  
🪲 Bug encontrado: botão “Delete” não funciona se o nome contém caracteres especiais.

---

## 5. Resumo de Achados

| ID | Descrição | Severidade | Status |
|----|------------|-------------|--------|
| UX01 | Campos obrigatórios sem destaque visual | Baixa | Aberto |
| UX02 | Clique direito não funcional em mobile | Média | Aberto |
| BUG01 | Botão “Delete” falha com caracteres especiais | Alta | Aberto |
| PERF01 | Alerta com atraso de mais de 5 segundos | Baixa | Aberto |

---

## 6. Sugestões de Melhoria
- Adicionar *feedback visual* nos campos obrigatórios.  
- Ajustar eventos de clique para compatibilidade com mobile.  
- Escapar caracteres especiais no cadastro da tabela.  
- Reduzir atraso no carregamento dos alertas.

---

## 7. Conclusão
O **DemoQA** apresenta boa estabilidade geral e cobre bem diferentes cenários para prática de QA manual.  
Foram identificadas **pequenas falhas de usabilidade e inconsistências pontuais**, úteis para fins de aprendizado e documentação.

---
