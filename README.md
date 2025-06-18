# 📊 Teste de Carga com Apache JMeter - API DummyJSON

Este projeto tem como objetivo realizar testes de carga e desempenho na API pública [DummyJSON](https://dummyjson.com), utilizando a ferramenta **Apache JMeter**.

---

## 📁 Estrutura do Projeto

.
├── outsera.jmx # Plano de teste JMeter
├── resultados.jtl # Arquivo de resultados gerado pela execução
├── report_html/ # Pasta gerada com o relatório em HTML
└── README.md # Este arquivo

## 🚀 Requisitos

- [Apache JMeter](https://jmeter.apache.org/) 5.6+
- Java 8+ (já configurado no JAVA_HOME)
- Terminal (bash, Git Bash, CMD ou PowerShell)

---

## ⚙️ Como Executar o Teste

1. **Executar o plano de teste:**

```bash
./jmeter -n -t outsera.jmx -l resultados.jtl
Gerar relatório HTML:

bash
Copiar
Editar
./jmeter -g resultados.jtl -o relatorio_html
Abrir o relatório:

Abra o arquivo relatorio_html/index.html em qualquer navegador.

🧪 O que está sendo testado
A API DummyJSON nos seguintes endpoints:

GET /products/

👥 Configuração do Teste
Usuários (threads): 500

Duração: 5 minutos

Ramp-up: 150 segundos

📈 Relatório Gerado
O relatório HTML inclui:

Gráficos de tempo de resposta

Taxa de throughput

Percentis (90%, 95%, 99%)

Erros por tipo

Visão geral por request

✨ Autor
Vinicios | Engenheiro de Qualidade de Software
Contato: LinkedIn (ou outro link)

📝 Licença
Este projeto é de uso livre para fins de aprendizado e testes.

---

Se quiser, posso:
- Inserir o README diretamente no seu `.jmx` como **documentação embutida**
- Adaptar para português técnico ou inglês, se for para GitHub internacional
- Incluir badges e GIFs de relatório automático

Deseja que eu gere o arquivo pronto pra colar no GitHub?