# LDA
Layered Data Architecture

## Arquitetura de Dados em Camadas

A Arquitetura de Dados em Camadas (ADC), visa acomodar os dados em seus diversos estágio de evolução sejam enquanto dados propriamente ditos ou enquanto transição para níveis de Informação, Conhecimento ou Sabedoria Organizacional.
Para tanto, a ADC define através de estágios de 0 a 5 o nível de maturidade, qualidade, organização e tipos de acesso que estão disponíveis.
Sinteticamente a ADC pode ser demonstrada da seguinte forma :


|   Nível   |   Estágio     |   Característica  |   DB Principal    |   DB Auxiliar |

| :-------------: |:-------------|: -----:|:------------- |:------------- |

|0  | Stick    | Extração, Captura, Disponibilidade e Tipagem | PostgreSQL | MongoDB|

| 1 | Stage    |  Limpeza, Qualidade, Enriquecimento | PostgreSQL | MongoDB|

| 2 | Facto      |    Regras, Indicadores, Fatos | PostgreSQL | MongoDB|

| 3 | Agreg     |   Agregações, Históricos, Dimensões| MongoDB| PostgreSQL |

| 4 | Expos  |    Dashboards, Relatórios, Fluxos, Arquivos  | ElasticSearch | Todos |

| 5 | Free      |   Área de trabalho Livre, Sandbox, Experimentação |  PostgreSQL | MongoDB |





![LDA Big Picture](/images/DataLayers-2.png?raw=true "LDA Big Picture")
