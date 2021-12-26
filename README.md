<div align="center">
  <h1>Modelo de Aprendizado de Máquina para identificação do comportamento da população na busca por serviços de saúde após o início da pandemia do novo coronavírus
</h1>
</div>



_________________




### Sobre
<a href="https://github.com/viniciusariza/comportamento-saude/blob/main/artigo/artigo.pdf">Artigo</a> e <a href="https://github.com/viniciusariza/comportamento-saude/blob/main/modelo"> código do modelo.</a>: Arquivos bloqueados, aguardando aprovação.
O modelo desenvolvido tem como objetivo aplicar um algoritmo classificador para identificar o comportamento da população na busca por serviços de saúde após o início da pandemia do novo coronavírus.

### Tecnologia
* Python

### Base de dados
A base de dados utilizada foi a Premise General Population Covid-19 Health Services Disruption Survey 2020, oriunda do projeto Covid-19 Health Services Disruption Survey 2020.

### Pré-processamento
* Seleção de atributos e instâncias
* Verificação de dados faltantes
* Imputação de dados em atributos quantitativos e qualitativos
* Codificação e binarização com Label Encoder e One Hot Encoder
* Normalização
* Over-sampling

<div align="center" >
  <img src="/img/pre-processamento.jpg">
</div>

### Métricas de avaliação
* Accuracy
* Precision
* Recall
* f1-score
* Confusion matrix

### Testes iniciais
* Naive Bayes
* Árvores de Decisão
* Random Forest
* Knn
* Regressão Logística
* Redes Neurais
* PCA
* Extra Trees
* Tuning de parâmetros
* Validação cruzada
* Teste de normalidade
* Teste de Turkey

### Modelo final
* Random Forest
* Ajuste de hiperparâmetros
* Validação cruzada (KFold)
* Análise e comparação
* Consolidação do modelo final

<div align="center" >
  <img src="/img/modelo.jpg">
</div>

### Conclusões
O modelo final apresentou acurácia de 88% com dados desconhecidos. Quanto à sensibilidade e a precisão, o modelo alcançou 0,89 em média, mostrando ser eficiente tanto na detecção de pessoas que buscaram cuidados médicos, quanto aqueles que não buscaram. A média harmônica entre a sensibilidade e a precisão foi de 0,88 para as duas classes. Com relação aos atributos mais importantes têm-se que se segue.

<div align="center" >
  <img src="/img/importancias.jpg">
</div>

Verificou-se que atributos sociodemográficos foram importantes na identificação da classe, sendo os mais influentes a quantidade de moradores em uma residência, a etnia, a religião e a situações empregatícia e financeira, cuja explicação pode ser consultada no <a href="https://github.com/viniciusariza/comportamento-saude/blob/main/artigo/artigo.pdf"> artigo completo.</a>
