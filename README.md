# Análise Exploratória de Dados - Corridas de Táxi em Chicago

Este projeto faz parte do meu portfólio e tem como objetivo explorar e analisar dados de corridas de táxi em Chicago durante novembro de 2017. O estudo utiliza Python para realizar análise exploratória, visualizações e testes de hipóteses, fornecendo insights valiosos que podem ser utilizados em estratégias de negócios.

---

## 📂 **Conjuntos de Dados Utilizados**
### 1. `/datasets/project_sql_result_01.csv`
- **Descrição**: Dados sobre o número de corridas para cada empresa de táxi entre 15 e 16 de novembro de 2017.
- **Colunas**:
  - `trips_amount`: Número de corridas para cada empresa de táxi.

### 2. `/datasets/project_sql_result_04.csv`
- **Descrição**: Dados sobre bairros de Chicago onde as corridas terminaram.
- **Colunas**:
  - `dropoff_location_name`: Nome do bairro de destino.
  - `average_trips`: Número médio de viagens que terminaram em cada bairro em novembro de 2017.

### 3. `/datasets/project_sql_result_07.csv`
- **Descrição**: Dados sobre viagens do Loop para o Aeroporto Internacional O'Hare.
- **Colunas**:
  - `start_ts`: Data e hora de coleta.
  - `weather_conditions`: Condições climáticas no início da corrida.
  - `duration_seconds`: Duração da corrida em segundos.

---

## 🎯 **Objetivos**
1. **Análise Exploratória**:
   - Importar e estudar os dados.
   - Verificar e ajustar os tipos de dados, se necessário.
   - Identificar os 10 principais bairros em termos de destinos.
   - Criar visualizações:
     - Empresas de táxi e número de corridas.
     - Top 10 bairros por número de corridas com destino nesses bairros.
   - Tirar conclusões baseadas nos gráficos.

2. **Teste de Hipóteses**:
   - **Hipótese**: "A duração média das corridas do Loop para o Aeroporto Internacional O'Hare muda nos sábados chuvosos."
   - Definir hipóteses nula e alternativa.
   - Escolher e aplicar o teste estatístico apropriado.
   - Explicar os resultados e conclusões.

---

## 📊 **Resultados**
### **Análise Exploratória**
1. **Top 10 Bairros em Termos de Destinos**:
   - Identificamos os bairros mais populares como destino de corridas. Essas informações podem ser utilizadas para campanhas de marketing ou estratégias de precificação.

2. **Empresas de Táxi e Número de Corridas**:
   - Observamos variações significativas entre empresas no número de corridas realizadas. Esse dado sugere a necessidade de análise de estratégias de mercado, como:
     - Apelo publicitário.
     - Segurança.
     - Preços e disponibilidade.
   - Uma análise SWOT seria útil para complementar essa avaliação.

### **Teste de Hipóteses**
- **Hipótese Nula (H₀)**: A duração média das corridas não muda em sábados chuvosos.
- **Hipótese Alternativa (H₁)**: A duração média das corridas muda em sábados chuvosos.
- **Critério Utilizado**: Teste t de Student (nível de significância: 0.05).
- **Resultado**:
  - Valor-p: `6.738994326108734e-12`
  - **Conclusão**: Rejeitamos a hipótese nula, confirmando que a duração média das corridas é diferente em sábados chuvosos.
  - **Média de Duração**:
    - Dias sem chuva: `1999.68 segundos`
    - Dias chuvosos: `2427.21 segundos`

---

## 🛠 **Ferramentas Utilizadas**
- Python
  - Pandas
  - Matplotlib
  - Seaborn
  - Scipy

---

## 📌 **Conclusões Gerais**
1. **Insights sobre os Bairros**:
   - Identificar bairros mais requisitados ajuda a planejar campanhas específicas ou ajustar preços para aumentar a lucratividade.

2. **Performance das Empresas**:
   - Analisar empresas com maior número de corridas pode revelar estratégias vencedoras no mercado.

3. **Impacto das Condições Climáticas**:
   - O aumento da duração das corridas em dias chuvosos pode ser considerado na gestão de preços e recursos.

---

## 📈 **Possibilidades de Expansão**
- Implementar análises adicionais como sazonalidade e impacto de eventos locais.
- Estender a análise para outros períodos ou regiões.
- Construir dashboards interativos para visualização dinâmica dos dados.

---

## 👨‍💻 **Contato**
Para mais informações ou feedback, entre em contato:
- **E-mail**: lara.danilo25@gmail.com
- **LinkedIn**: [Danilo](https://www.linkedin.com/in/danilojosedelara/)
