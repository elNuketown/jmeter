# 📊 Teste de Carga com Apache JMeter - API DummyJSON

Este projeto realiza testes de carga e desempenho na API pública [DummyJSON](https://dummyjson.com), utilizando a ferramenta **Apache JMeter**.

---

## 📁 Estrutura do Projeto

- `teste.jmx` – Plano de teste configurado no JMeter  
- `resultados.jtl` – Arquivo de saída com os resultados do teste  
- `reporte_html/` – Relatório completo em HTML gerado a partir dos resultados  
- `README.md` – Documentação do projeto

---

## ⚙️ Requisitos

- [Apache JMeter 5.6+](https://jmeter.apache.org/)
- Java 8 ou superior (com `JAVA_HOME` configurado)
- Terminal Bash, Git Bash, PowerShell ou CMD

---

## 🚀 Executando os Testes

**1. Rodar o teste em modo não-GUI:**

./jmeter -n -t teste.jmx -l resultados.jtl

**2. Gerar o reporte:**

./jmeter -g resultado.jtl -o reporte_html

**3. Visualizar report:**

Abra o arquivo reporte/index.html em seu navegador.

---

## 🚀 Configuração do projeto

- Número de usuários (threads): 500

- Duração do teste: 5 minutos

- Ramp-up: 150 segundos

---

## 🚀 Relatorio HTML 

- Tempo médio e máximo de resposta

- Gráficos de throughput e tempo por segundo

- Percentis (90%, 95%, 99%)

- Tabela de erros por request

- Métricas por amostra de requisição

---

## 🚀 Autor

Vinicios Virissimo

---