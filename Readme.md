# 🚒 Projeto KNIME – Análise de Ocorrências de Bombeiros, Condições Meteorológicas e Veículos


## Enquadramento
Este projeto foi desenvolvido no âmbito da Unidade Curricular **Engenharia de Sistemas de Informação (ESI-ISI)**, com o objetivo de aplicar técnicas de **ETL (Extract, Transform, Load)** utilizando a ferramenta **KNIME**.  
O tema escolhido foi **“Ocorrências de Bombeiros”**, relacionando tipos de ocorrências (incêndios, emergências, acidentes, etc.) com dados meteorológicos (temperatura, vento e precipitação) e veículos.

---

## Estrutura do Projeto
O workflow está organizado em **três componentes principais**, que representam as fases do processo ETL:

### Input Data Component
- **Objetivo:** Leitura e extração de dados de diferentes fontes (CSV, JSON e XML).  
- **Principais nós:** CSV Reader, JSON Reader, JSON Path, Ungroup, XPath, String to Date&Time, Number to String.  
- **Descrição:** Extrai e estrutura dados de ocorrências e meteorologia, convertendo tipos e normalizando formatos para integração posterior.

### Data Processing Component
- **Objetivo:** Transformação, integração e agregação dos dados.  
- **Principais nós:** String Manipulation (com Regex), Rule Engine, Joiner, GroupBy, String to Number...  
- **Descrição:** Realiza limpeza e normalização dos dados, integração entre ficheiros (por data e local), e cálculo de médias e estatísticas.  

### Output & Visualization Component
- **Objetivo:** Visualizar e exportar resultados.  
- **Principais nós:** Bar Chart, Scatter Plot, CSV Writer, Excel Writer, DB Writer, SQLite Connector, Java Snippet.  
- **Descrição:** Gera gráficos de análise, exporta dados processados e armazena resultados em ficheiros e base de dados SQLite.

---

## Funcionalidades Implementadas
- **Expressões Regulares (Regex)** para normalização de texto.  
- **Integração de dados** de múltiplas fontes (CSV, JSON e XML).  
- **Operações de transformação:** Joiner, GroupBy, Missing Value, Sorter, Row Filter.  
- **Exportação e persistência de dados** (CSV, Excel, Base de Dados SQLite).  
- **Visualização de resultados:** Bar Chart (tempo médio por tipo de ocorrência) e Scatter Plot (aplicação vs veículos).  
- **Geração de logs automáticos** com Java Snippet.

---

## Exemplos de Visualizações
- **Bar Chart:** Tempo médio de resposta por tipo de ocorrência.  
- **Scatter Plot:** Relação aplicação e veículos ativos.  


---


## Como Executar
1. Abrir o ficheiro `.knwf` no KNIME Analytics Platform.  
2. Confirmar os caminhos dos ficheiros CSV, JSON e XML nos nós de leitura.  
3. Executar os três componentes pela ordem:
   - **Input Data Component**
   - **Data Processing Component**
   - **Output & Visualization Component**
4. Visualizar os gráficos no Bar Chart e Scatter Plot.  
5. Verificar os resultados exportados (CSV, Excel e SQLite).

---

## Resultados Esperados
- Média do tempo de resposta por tipo de ocorrência.  
- Relação entre aplicação de veículos e veículos ativos.  
- Base de dados consolidada e limpa.  
- Geração automática de logs de execução.

---

## Ferramentas e Tecnologias
- **KNIME Analytics Platform**  
- **SQLite**  
- **CSV, JSON e XML**  
- **Java (via Java Snippet)**

---

## Equipa
- **Aluno:** Nuno Miguel Rodrigues da Silva  
- **Curso:** Engenharia de Sistemas Informáticos
- **Unidade Curricular:** Integração de Sistemas de Informação  
- **Ano Letivo:** 2025/2026  

