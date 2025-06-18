# 📊 Teste de Carga com Apache JMeter - API DummyJSON

Este projeto realiza testes de carga e desempenho na API pública [DummyJSON](https://dummyjson.com), utilizando a ferramenta **Apache JMeter**.

---

## 📁 Estrutura do Projeto

- `outsera.jmx` – Plano de teste configurado no JMeter  
- `resultados.jtl` – Arquivo de saída com os resultados do teste  
- `relatorio_html/` – Relatório completo em HTML gerado a partir dos resultados  
- `README.md` – Documentação do projeto

---

## ⚙️ Requisitos

- [Apache JMeter 5.6+](https://jmeter.apache.org/)
- Java 8 ou superior (com `JAVA_HOME` configurado)
- Terminal Bash, Git Bash, PowerShell ou CMD

---

## 🚀 Executando os Testes

**1. Rodar o teste em modo não-GUI:**

```bash
./jmeter -n -t outsera.jmx -l resultados.jtl

---

2. Gerar o relatório HTML:

```bash
./jmeter -g resultados.jtl -o relatorio_html
