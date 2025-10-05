# 🧩 Plano de Teste – SauceDemo

## 1. Introdução
Este plano de teste tem como objetivo validar o funcionamento das principais funcionalidades da aplicação **[SauceDemo](https://www.saucedemo.com/)**, um e-commerce de demonstração usado para práticas de QA.

O foco está nos fluxos de **login**, **navegação de produtos**, **adição ao carrinho** e **finalização de compra**.

---

## 2. Escopo
**Incluído:**
- Login com credenciais válidas e inválidas
- Listagem de produtos
- Adição e remoção de produtos no carrinho
- Finalização de compra

**Excluído:**
- Testes de performance
- Testes de integração com backend
- Testes automatizados

---

## 3. Tipos de Teste
- Teste funcional
- Teste de regressão
- Teste exploratório

---

## 4. Ambiente de Teste
- **URL:** https://www.saucedemo.com/  
- **Navegador:** Google Chrome 128  
- **Sistema Operacional:** Windows 10  
- **Resolução:** 1920x1080  

---

## 5. Critérios de Aceite
- Todos os casos críticos devem passar.
- Nenhum bug de severidade alta deve permanecer aberto.
- As mensagens e fluxos devem seguir o comportamento esperado da interface.

---

## 6. Cronograma
| Etapa | Data | Responsável |
|--------|------|-------------|
| Planejamento | 05/10/2025 | Izabela Andrade |
| Execução dos testes | 05/10/2025 | Izabela Andrade |
| Registro de bugs e relatório final | 06/10/2025 | Izabela Andrade |

---

## 7. Riscos e Mitigações
| Risco | Impacto | Mitigação |
|--------|----------|------------|
| Instabilidade do site | Alto | Repetir teste em outro horário |
| Erro de ambiente | Médio | Registrar no relatório e revalidar |
| Dados não persistentes | Baixo | Recriar sessão antes de retestar |

---

## 8. Entregáveis
- Plano de teste (este documento)
- Casos de teste (test-cases.md)
- Relatório de bugs (bug-reports.md)
- Evidências em formato de imagem (.png)
