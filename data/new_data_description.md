# Dicionário de Dados - Dataset Final (Ames Housing Modificado)

**NOTA IMPORTANTE:**
Com exceção da variável alvo (`Preco_Venda`), **todas** as demais 39 variáveis passaram por um processo de padronização (`StandardScaler`). Isso significa que os "Valores Possíveis" mostrados na tabela abaixo foram transformados pelo algoritmo para uma escala de média 0 e desvio padrão 1 (ex: valores como `1500`, `3` ou `1` viraram números proporcionais como `1.04`, `-0.33`, etc).

| Variável | Valores Possíveis (Originais) | Categoria | Normalizada? | Descrição |
| :--- | :--- | :--- | :---: | :--- |
| **Preco_Venda** | Valores Contínuos | Alvo (Target) | **Não** | Preço final de venda da propriedade em dólares. |
| **Area_Total_Construida** | Valores Contínuos | Nova Feature | Sim | Soma das áreas do porão, 1º e 2º andar (em pés quadrados). |
| **Total_Banheiros** | `0, 0.5, 1, 1.5, 2...` | Nova Feature | Sim | Número de banheiros (Completos valem 1, lavabos valem 0.5). |
| **Idade_Imovel_Venda** | `0, 1, 2, 3...` | Nova Feature | Sim | Anos de vida do imóvel no exato momento da venda. |
| **Idade_Reforma_Venda** | `0, 1, 2, 3...` | Nova Feature | Sim | Anos desde a última reforma no exato momento da venda. |
| **Area_Habitavel_Acima_Solo** | Valores Contínuos | Numérica Contínua | Sim | Área de convivência acima da superfície (exclui porão). |
| **Area_Total_Porao** | Valores Contínuos | Numérica Contínua | Sim | Área total do porão em pés quadrados. |
| **Area_Primeiro_Andar** | Valores Contínuos | Numérica Contínua | Sim | Área do primeiro andar em pés quadrados. |
| **Area_Segundo_Andar** | Valores Contínuos | Numérica Contínua | Sim | Área do segundo andar em pés quadrados. |
| **Area_Garagem** | Valores Contínuos | Numérica Contínua | Sim | Tamanho da garagem em pés quadrados. |
| **Fachada_Lote_Pes** | Valores Contínuos | Numérica Contínua | Sim | Pés lineares de rua conectados à fachada da casa. |
| **Area_Alvenaria** | Valores Contínuos | Numérica Contínua | Sim | Área do revestimento de alvenaria/pedra. |
| **Area_Acab_Porao1** | Valores Contínuos | Numérica Contínua | Sim | Área finalizada/acabada do porão tipo 1. |
| **Area_Deck_Madeira** | Valores Contínuos | Numérica Contínua | Sim | Tamanho do deck de madeira externo. |
| **Area_Varanda_Aberta** | Valores Contínuos | Numérica Contínua | Sim | Tamanho da varanda aberta externa. |
| **Capacidade_Carros_Garagem** | `0, 1, 2, 3, 4` | Numérica Discreta | Sim | Capacidade da garagem em quantidade de carros. |
| **Total_Comodos_Acima_Solo** | `0, 1, 2, 3...` | Numérica Discreta | Sim | Número total de cômodos na casa (não inclui banheiros). |
| **Banheiros_Completos** | `0, 1, 2, 3...` | Numérica Discreta | Sim | Número de banheiros completos acima do solo. |
| **Lareiras** | `0, 1, 2, 3` | Numérica Discreta | Sim | Número de lareiras existentes na casa. |
| **Ano_Construcao_Garagem** | Anos (Ex: `1990`) | Numérica Discreta | Sim | Ano original de construção da garagem. |
| **Qualidade_Geral** | `1` a `10` | Categórica Ordinal | Sim | Nota geral de qualidade dos materiais e acabamento. |
| **Qualidade_Externa** | `0` a `5` | Categórica Ordinal | Sim | Avaliação da qualidade do revestimento externo. |
| **Qualidade_Cozinha** | `0` a `5` | Categórica Ordinal | Sim | Avaliação da qualidade da cozinha. |
| **Qualidade_Porao** | `0` a `5` | Categórica Ordinal | Sim | Avaliação da altura/qualidade do porão. |
| **Qualidade_Aquecimento**| `0` a `5` | Categórica Ordinal | Sim | Condição e qualidade do sistema de aquecimento. |
| **Qualidade_Piscina** | `0` a `5` | Categórica Ordinal | Sim | Qualidade da piscina (`0` para casas sem piscina). |
| **Exposicao_Porao** | `0` a `4` | Categórica Ordinal | Sim | Avaliação de acesso de saída para o exterior. |
| **Acabamento_Garagem** | `0` a `3` | Categórica Ordinal | Sim | Nível de acabamento interno da garagem. |
| **Bairro_NridgHt** | `0` ou `1` | Categórica Binária | Sim | Se a casa está no bairro Northridge Heights. |
| **Bairro_NoRidge** | `0` ou `1` | Categórica Binária | Sim | Se a casa está no bairro Northridge. |
| **Tipo_Fundacao_PConc** | `0` ou `1` | Categórica Binária | Sim | Fundação de Concreto Moldado (*Poured Concrete*). |
| **Tipo_Fundacao_CBlock** | `0` ou `1` | Categórica Binária | Sim | Fundação de Bloco de Concreto (*Cinder Block*). |
| **Classe_Imovel_60** | `0` ou `1` | Categórica Binária | Sim | Se a casa é de 2 andares estilo pós-1946. |
| **Tipo_Venda_New** | `0` ou `1` | Categórica Binária | Sim | Se a venda é de uma casa nova/recém-construída. |
| **Condicao_Venda_Partial**| `0` ou `1` | Categórica Binária | Sim | Se a transação é parcial (comum em casas Novas). |
| **Tipo_Garagem_Attchd** | `0` ou `1` | Categórica Binária | Sim | Garagem conectada fisicamente à casa. |
| **Tipo_Garagem_Detchd** | `0` ou `1` | Categórica Binária | Sim | Garagem em estrutura separada da casa. |
| **Tipo_Alvenaria_Stone** | `0` ou `1` | Categórica Binária | Sim | Revestimento de alvenaria em Pedra. |
| **Revestimento_Externo1_VinylSd**| `0` ou `1` | Categórica Binária | Sim | Revestimento primário em Vinil. |
| **Revestimento_Externo2_VinylSd**| `0` ou `1` | Categórica Binária | Sim | Revestimento secundário em Vinil. |
