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
| Prevenção de erros | A interface deve evitar erros do usuário | Campo Date of Birth aceita datas futuras |
| Estética e design minimalista | A tela deve ser limpa e intuitiva | Alguns elementos estão sobrepostos em telas pequenas |

---

## 4. Cenários Testados

### Cenário 1 – Validação de campo “Date of Birth”
**Passos:**
1. Acessar o formulário “Practice Form”.  
2. Clicar no campo **“Date of Birth”**.  
3. Selecionar uma data **futura** (ex: 10/10/2030).  
4. Preencher os demais campos obrigatórios.  
5. Enviar o formulário.  

**Resultado esperado:**  
- O sistema **deve impedir** a seleção de datas futuras e mostrar mensagem de erro.  

**Resultado obtido:**  
- O sistema **permite** enviar o formulário com data futura sem qualquer validação.  

**Status:** ❌ Falha  
**Severidade:** Média  
**Prioridade:** Alta  
**Evidência:** *https://ibb.co/prd24fHD*

---

### Cenário 2 – Botões de Ação
**Passos:**
1. Acessar página “Buttons”.  
2. Clicar uma vez, duplo clique e clique com o botão direito.  

**Resultado esperado:**  
- Cada tipo de clique exibe a mensagem correspondente.  

**Resultado obtido:**  
✅ Funciona corretamente no desktop.  
⚠️ Clique direito não funciona no mobile.

---

### Cenário 3 – Tabelas Interativas
**Passos:**
1. Acessar página “Web Tables”.  
2. Adicionar, editar e excluir registros.  

**Resultado esperado:**  
- Tabela atualiza conforme ações.  

**Resultado obtido:**  
✅ Edição e exclusão funcionam corretamente.  
🪲 Bug: botão “Delete” não funciona corretamente com caracteres especiais, este deleta 3 registros ao invés de apenas o selecionado.

---

## 5. Resumo de Achados

| ID | Descrição | Severidade | Status |
|----|------------|-------------|--------|
| UX01 | Campo Date of Birth permite datas futuras | Média | Aberto |
| UX02 | Clique direito não funcional em mobile | Média | Aberto |
| BUG01 | Botão “Delete” falha com caracteres especiais | Alta | Aberto |

---

## 6. Sugestões de Melhoria
- Bloquear datas futuras no campo Date of Birth.  
- Corrigir clique direito para mobile.  
- Corrigir botão Delete com caracteres especiais.  

---

## 7. Conclusão
O **DemoQA** apresenta boa estabilidade geral e cobre bem diferentes cenários para prática de QA manual. Foram identificadas **pequenas falhas funcionais e de usabilidade**, relevantes para aprendizado e documentação.
