# Precificação de Imóveis com Aprendizagem de Máquina e Dados do Censo

## Introdução

Este trabalho aborda a precificação de imóveis com o uso de modelos de Aprendizagem de Máquina. Para tal, foram usadas bases de dados com características dos imóveis e bases do Censo de 2010 que, por meio de diferentes técnicas de geolocalização, fornecem informações sobre a região dos imóveis.

## Motivação: por que precificar imóvel? Para que serve? Quais os desafios?

Precificar um imóvel é um desafio enfrentado por muitas empresas e isso é usado para diversas finalidades. As imobiliárias necessitam disso, pois são focadas na compra e venda de imóveis. Os bancos, que retomam os imóveis de financiadores inadimplentes ou que precisam precificar o imóvel de garantia do cliente para gerar um score de crédito e, até mesmo, as empresas focadas exclusivamente nessa precificação.

A precificação de um imóvel depende de diversos fatores, como metragem quadrada, preço do metro quadrado na região, número de quartos, banheiros, vagas de garagem, geolocalização etc.

Com base em tantos fatores, é um desafio para as empresas fazer uma precificação assertiva. E o erro na estimativa de preço de um imóvel é um problema por vários motivos. Por exemplo, para quem está vendendo, sobrestimar o preço pode causar uma demora demasiada na venda do imóvel, ao passo que subestimá-lo causará a venda abaixo do preço ideal, gerando uma diminuição da receita.

## Estrutura do projeto

O projeto é composto por 5 etapas principais:


Todas as etapas contribuíram para o bom desempenho do modelo final, mas vale um destaque para engenharia de atributos. Depois da inclusão dos dados do Censo, da criação e da expansão de atributos, o percentual de acerto da precificação aumentou significativamente.

## Resultados obtidos

O tipo de avaliação dos modelos depende do contexto da precificação. Então, supondo que estamos do lado dos vendedores de imóveis, é menos prejudicial sobrestimar o preço pois, tendo esse tipo de erro, basta implementar um desconto no preço do imóvel a cada período de tempo ou a cada número de tentativas frustradas de venda. Portanto, para avaliar os modelos, foi criada seguinte métrica de avaliação:

Com isso, os modelos tiveram uma tolerância maior ao erro de sobrestimar o preço ($20\%$) do que ao erro de subestimar ($10\%$). Os resultados obtidos foram os seguintes:

Por fim, o melhor resultado obtido foi $100\%$ de acerto.

## Referências

\begin{thebibliography}{99}
\bibitem{este livro} HARRISON, Matt. \textbf{Machine Learning:}  Guia de Referência Rápida. São Paulo - SP, Brasil: novatec, 2020.
