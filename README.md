## Dashboard de produção





### 🔧 Ferramentas
- Excel
  
- Power BI

### 📝 Skills utilizadas
- Limpeza de dados

- Tratamento de dados

- Coleta de informações

- transformação das informações em insights

## 🔗 Etapas

### 🔗 Extração
Essa tabela do excel é pública e foi retirada do site kaggle

### 🔗 Trasnformação / Limpeza
- Trasnformação
  Para a transformação foi preciso adicionar 7 medidas que foram:

### HORAS PRODUZIDA
HORAS PRODUZIDAS = CALCULATE(SUM('BASEPRODUÇÃO'[TOTAL HORAS]), 'BASEPRODUÇÃO'[OCORRÊNCIA]=BLANCK())

### HORAS PARADAS
HORAS PARADAS = CALCULATE(SUM('BASEPRODUÇÃO'[TOTAL HORAS]), 'BASEPRODUÇÃO'[OCORRÊNCIA]<>BLANCK())

### HORAS
HORAS = SUM('BASEPRODUÇÃO'[TOTAL HORAS])

### DISPONIBILIDADE
DISPONIBILIDADE = ([HORAS PRODUZIDAS])/(HORAS PRODUZIDAS] + [HORAS PARADAS])

### QUANTIDADE PRODUZIDA
QUANT.PRODUZIDA = SUM('BASEPRODUÇÃO'[QTDPRODUZIDA])

### QUANTIDADE REJEITADA
QUANT. REJEITADA = SUM('BASEPRODUÇÃO'[QTD REJEITADA]

### QUALIDADE
QUALIDADE = ([QUANT. PRODUZIDA])/([QUANT. PRODUZIDA] + [QUANT.REJEITADA])


### 🔗 Análise
Iniciei com o processo de análise exploratória, buscando uma visão geral dos dados, verificando dados faltantes ou duplicados, distribuição e tipos, dados em brancos.

Depois disso fui para a criação do dasboard
### 1° passo
- Foi criado
4 cartões de linha múltipla 
1 gráfico de área
2 gráficos de velocímetro 
1 cartão de segmentação de dados

### 2° passo
- adicionando imagens.
Depois dos gráficos criados entrei no site www.flaticon.com e baixei algumas imagens para adicionar nos gráficos de cartões de linha múltiplas.

### 🔗 Resultados das análises

Após finalizado foi possível destacar os seguintes insights:

1° Quantidade produzida
2° Quantidade rejeitada
3° Horas produtivas
4° Horas paradas
5° Destacar a produção de cada operador
6° A produção mensal
7° Mostra a porcentagem da disponibilidade
8° Mostra a porcentagem da qualidade.

### Com tudo, é possível acompanhar os resultados de cada funcionário, acompanhando sua projeção mensal, acompanhando o desenvolvimento de cada colaborador.

### 🔗 Teste as funções online:https://app.powerbi.com/view?r=eyJrIjoiMDAzOTA3OTctM2ZiNi00ODFiLWJiZDEtMTcwYmVjYTA3OGE5IiwidCI6ImQ1NTZmMWRlLTA1ZDMtNDNiZC1iMGMyLTIzODY4ZWEyNGFlNSJ9
