📊 Teste de Carga com Apache JMeter - API DummyJSON
Este projeto realiza testes de carga e desempenho na API pública DummyJSON, utilizando a ferramenta Apache JMeter.

📁 Estrutura do Projeto
outsera.jmx – Plano de teste configurado no JMeter

resultados.jtl – Arquivo de saída com os resultados do teste

relatorio_html/ – Relatório completo em HTML gerado a partir dos resultados

README.md – Documentação do projeto

⚙️ Requisitos
Apache JMeter 5.6+

Java 8 ou superior (com JAVA_HOME configurado)

Terminal Bash, Git Bash, PowerShell ou CMD

🚀 Executando os Testes
1. Rodar o teste em modo não-GUI:

bash
Copiar
Editar
./jmeter -n -t outsera.jmx -l resultados.jtl
2. Gerar o relatório HTML:

bash
Copiar
Editar
./jmeter -g resultados.jtl -o relatorio_html
3. Visualizar o relatório:

Abra o arquivo relatorio_html/index.html em seu navegador.

🧪 Endpoints Testados
GET /products/1

POST /products/add

PUT /products/1

DELETE /products/1

Todos os endpoints são da API DummyJSON e foram configurados com payloads de teste para simular um fluxo completo de uso da aplicação.

👥 Configuração do Teste
Número de usuários (threads): 500

Duração do teste: 5 minutos

Ramp-up: 300 segundos

Validações: Códigos HTTP e conteúdo da resposta (Assertions)

📈 Sobre o Relatório HTML
O relatório inclui:

Tempo médio e máximo de resposta

Gráficos de throughput e tempo por segundo

Percentis (90%, 95%, 99%)

Tabela de erros por request

Métricas por amostra de requisição

👨‍💻 Autor
Vinicios Virissimo
Engenheiro de Qualidade de Software
📫 LinkedIn (substitua pelo seu perfil real)

📝 Licença
Este projeto é livre para fins de estudo, aprendizado e demonstração de testes de carga com JMeter.