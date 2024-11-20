# Em relação ao dataset vgsales.csv

Esse dataset foi baixado do site da Kaggle: Your Home for Data Science.

Os dados contêm informações de duas décadas de vendas de games no mundo.
Escolhi esses dados, por ser um grande consumidor do mercado.

Explicação em relação ao que foi feito nesse dataset.

## 1.Pré-processamento
Removemos valores NaN, nulos das colunas Year, Publisher.
Removemos também os valores 0.00 e 0.0 das colunas de vendas que estavam alterados a modelagem.
e análise exploratória.
Conversão da coluna Year de float para integer
As colunas não renomeadas estão em inglês e portuges :( , futuramente correção).

## 2. Modelagem 
XGBoost por ser um bom algoritmo para esse dataset e para o que precisava.
Transformamos as colunas categorias para numéricas.
***IMPORTATNE***
Criei features para melhorar na modelagem, então mesclei as colunas de vendas.
Criando uma coluna região e valores dessa mesma região.
Criei as colunas Year_Category, Rank_Category

## 3. Avalição e Métricas
Acuracidade e um relatório dessa métrica foi ótimo! Porém, irei usar outras métricas.<br>
O resultado foi  Acurácia do modelo: 0.86 padrão.<br>
Acurácia: 85.91%  


 
