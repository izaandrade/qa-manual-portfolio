# 🪲 Relatórios de Bugs – DemoQA

---

### Bug 01 – Campo Date of Birth permite datas futuras
- **Severidade:** Média  
- **Status:** Aberto  
- **Ambiente:** Windows 11 Home, Chrome  
- **Passos para reproduzir:**
  1. Acessar o formulário “Practice Form” em [DemoQA Forms](https://demoqa.com/automation-practice-form)  
  2. Clicar no campo **Date of Birth**  
  3. Selecionar uma data futura (ex: 10/10/2030)  
  4. Preencher os demais campos obrigatórios  
  5. Enviar o formulário  
- **Resultado esperado:** Sistema deve impedir datas futuras e exibir mensagem de erro  
- **Resultado obtido:** Formulário é enviado com data futura sem qualquer validação  
- **Evidência:** *(https://ibb.co/prd24fHD)*

---

### Bug 02 – Clique direito não funcional no mobile
- **Severidade:** Média  
- **Prioridade:** Média  
- **Status:** Aberto  
- **Ambiente:** Smartphone IOS, Safari  
- **Passos para reproduzir:**
  1. Acessar página “Buttons” em [DemoQA](https://demoqa.com/buttons)  
  2. Tentar realizar um **clique com o botão direito**  
- **Resultado esperado:** Mensagem correspondente ao clique direito deve aparecer  
- **Resultado obtido:** Clique direito não gera nenhuma resposta
