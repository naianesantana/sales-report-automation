# 🤖 Automação de Relatório Diário de Vendas via E-mail

> ⚠️ **Status do Projeto:** ✅ *Finalizado!*

Uma solução de automação de processos (RPA) desenvolvida em Python para otimizar o fluxo de rotina de análise de dados diária. 

O objetivo do projeto é automatizar a extração das métricas de vendas do dia anterior (faturamento e quantidade de produtos) atualizadas pelo sistema e realizar o envio diário do relatório diretamente para a diretoria por e-mail.

---

## 📌 Contexto do Problema

Diariamente, o sistema corporativo atualiza as vendas realizadas no dia anterior. Como analista de dados, a primeira tarefa da rotina de trabalho consiste em consultar essas atualizações, consolidar as métricas principais e reportá-las à diretoria via e-mail.

A execução manual dessa rotina consome tempo e está sujeita a atrasos ou erros operacionais. Este projeto visa eliminar a intervenção humana nessa tarefa repetitiva.

---

## 🛠️ Tecnologias e Bibliotecas Utilizadas

* **Python 3.14.2** - Linguagem base do projeto
* **PyAutoGUI** - Automação de comandos do mouse e teclado (RPA)
* **Pandas** - Manipulação e análise dos dados de vendas
* **Jupyter Notebook** *(VS Code)* - Ambiente de desenvolvimento e execução dos testes

---

## 🚀 Fluxo de Execução da Automação

O projeto foi estruturado em 5 etapas principais que simulam o comportamento humano do analista:

1. **Acesso ao Sistema:** Abertura do navegador e navegação até o sistema corporativo (Google Drive).
2. **Navegação na Base de Dados:** Localização e seleção da pasta com os arquivos atualizados de vendas.
3. **Download dos Dados:** Download automático do arquivo de dados para o ambiente local.
4. **Cálculo de Indicadores:** Leitura do arquivo extraído via Pandas para calcular:
   * **Faturamento Total** do dia anterior.
   * **Quantidade Total** de produtos vendidos.
5. **Report à Diretoria:** Abertura do e-mail e envio automatizado do relatório consolidado com os indicadores calculados.

---

## 📋 Como Executar o Projeto

### Pré-requisitos
Certifique-se de ter o Python instalado e as dependências listadas abaixo:

```bash
pip install pyautogui pandas openpyxl
