# Machine Learning Engineer Nanodegree
## Proposta do projeto de conclusão
Leandro Humberto Vieira

## Aplicação de machine learning e visão computacional na extração de informação sobre roupas femininas

### Descrição do domínio

  A imagem é a primeira impressão que uma pessoa tem ao ver alguém, é algo que nosso cérebro faz automaticamente para armazenar informações e é realizado a partir do momento em que começamos a interagir com esta pessoa. Uma imagem diferente do que uma pessoa é durante uma conversa causa um "ruído" na comunicação e uma confusão no nosso cérebro.
 
  Hoje a imagem é uma via de comunicação pessoal tão importante quanto a fala, dessa forma surgiu a necessidade de profissionais que ensinam a arte da comunicação não-verbal, através de métodos e análises que permitem ensinar uma pessoa a se conhecer e, assim, expressar melhor seu estilo e personalidade através de sua imagem. O processo de [consultoria de imagem](https://en.wikipedia.org/wiki/Image_consulting) ensina a pessoa a identificar seu estilo e sua personalidade, e após este passo, trabalhar com o objetivo de construir uma imagem pessoal mais positiva e coerente com a cliente.
  A consultoria de imagem trabalha em sua grande parte com roupas, logo há algumas etapas que visam limpar, organizar e classificar as roupas da cliente(assim como os cientistas de dados fazem com dados).
  
### Por que a consultoria de imagem é importante

A imagem, o estilo e as vestimentas sao fatores que regem ou influenciam vários aspectos da vida de uma pessoa, o que torna esta informação muito valiosa e digna de vários estudos como os descritos abaixo:

* [Como a roupa afeta sua consciência](http://www.dailymail.co.uk/sciencetech/article-2644076/You-DRESS-Clothing-significant-effect-self-esteem-confidence-claims-expert.html) Livro:https://www.amazon.com/Mind-What-You-Wear-Psychology-ebook/dp/B00KBTB3NS/ref=sr_1_1?ie=UTF8&qid=1454635783&sr=8-1&keywords=Mind+What+You+Wear

* [Como a roupa impacta no seu sucesso profissional](http://www.businessinsider.com/how-your-clothing-impacts-your-success-2014-8)
* [A correlação da vestimenta com o relacionamento](https://www.meetmindful.com/the-way-you-dress/)
* [Benefícios da organização das roupas](https://www.janeisatomas.com.br/6-vantagens-de-ter-um-closet-organizado/)

  Optei por este desafio pois [minha esposa](https://www.instagram.com/karinataniaconsultoria/?hl=pt-br) é consultora de imagem há 1 ano e tem como especialidades o **atendimento online** e uma metodologia de [como montar um armário inteligente](https://www.youtube.com/watch?v=QSFPt3cG6CQ&t=2340s). Desejo apoiá-la neste assunto, utilizando tecnologia para dar vantagem competitiva ao produto dela, tornando o processo de transformação do armário mais interativo, automatizado e divertido.
  
### Descrição do problema

O problema a ser resolvido se define em como ter uma visão estratégica do armário de uma mulher. Apenas olhando para o armário, por mais organizado que esteja, não é possível responder perguntas como:

* Quantas blusas pretas eu tenho?
* Quais são as peças que faltam no armário?
* Qual a proporção casual/trabalho que tenho?





In this section, clearly describe the problem that is to be solved. The problem described should be well defined and should have at least one relevant potential solution. Additionally, describe the problem thoroughly such that it is clear that the problem is quantifiable (the problem can be expressed in mathematical or logical terms) , measurable (the problem can be measured by some metric and clearly observed), and replicable (the problem can be reproduced and occurs more than once).

### Dados de entrada
_(approx. 2-3 paragraphs)_

Os dados de entrada foram pesquisados na internet e dois candidatos possuem um excelente encaixe na solução: 

## [Fashion MNIST](https://github.com/zalandoresearch/fashion-mnist)

  O Fashion MNIST é um conjunto de dados criado pela [Zalando Research](https://research.zalando.com/), que contém 60 mil imagens de roupas no conjunto de treino e outras 10 mil no conjunto de teste. Este conjunto de dados tem como objetivo principal substituir o [MNIST](http://yann.lecun.com/exdb/mnist/), pois o mesmo é um conjunto que [não condiz com a realidade dos problemas de Deep Learning](https://twitter.com/fchollet/status/852592598128615424)

## [Apparel classification with Style](http://www.vision.ee.ethz.ch/~lbossard/projects/accv12/index.html)

  O Apparel classification Set contém imagens retiradas da web através de crawlers e já classificadas em 15 grupos diferentes de categorias de roupa. Os dados deste conjunto são muito mais semelhantes com a realidade da aplicação final, pois mostram as roupas vestidas em pessoas em lugares naturais.



In this section, the dataset(s) and/or input(s) being considered for the project should be thoroughly described, such as how they relate to the problem and why they should be used. Information such as how the dataset or input is (was) obtained, and the characteristics of the dataset or input, should be included with relevant references and citations as necessary It should be clear how the dataset(s) or input(s) will be used in the project and whether their use is appropriate given the context of the problem.

### Descrição da solução

A solução envolve a construção de um aplicativo mobile que permitirá uma pessoa gerenciar seu armário com mais facilidade, através da construção de um "armário virtual". O processo consiste de um cadastro inicial, indicando a quantidade de peças que a pessoa possui no armário. Após isso o aplicativo iniciará como um armário vazio, e ele será preenchido organicamente pela cliente, através de fotos com o "look do dia". Com as fotos, é o trabalho da solução classificar as roupas utilizadas nas fotos e adicioná-las ao armário virtual, com o devido cuidado de não criar a peça duplicadamente no armário.
  Com a geração destes dados classificados, utilizá-los para mostrar estatísticas descritivas e prescritivas do armário para a cliente.

### Modelo de comparação
_(approximately 1-2 paragraphs)_

In this section, provide the details for a benchmark model or result that relates to the domain, problem statement, and intended solution. Ideally, the benchmark model or result contextualizes existing methods or known information in the domain and problem given, which could then be objectively compared to the solution. Describe how the benchmark model or result is measurable (can be measured by some metric and clearly observed) with thorough detail.

### Métrica de validação
_(approx. 1-2 paragraphs)_

In this section, propose at least one evaluation metric that can be used to quantify the performance of both the benchmark model and the solution model. The evaluation metric(s) you propose should be appropriate given the context of the data, the problem statement, and the intended solution. Describe how the evaluation metric(s) are derived and provide an example of their mathematical representations (if applicable). Complex evaluation metrics should be clearly defined and quantifiable (can be expressed in mathematical or logical terms).

### Design do projeto
_(approx. 1 page)_

In this final section, summarize a theoretical workflow for approaching a solution given the problem. Provide thorough discussion for what strategies you may consider employing, what analysis of the data might be required before being used, or which algorithms will be considered for your implementation. The workflow and discussion that you provide should align with the qualities of the previous sections. Additionally, you are encouraged to include small visualizations, pseudocode, or diagrams to aid in describing the project design, but it is not required. The discussion should clearly outline your intended workflow of the capstone project.

-----------

**Before submitting your proposal, ask yourself. . .**

- Does the proposal you have written follow a well-organized structure similar to that of the project template?
- Is each section (particularly **Solution Statement** and **Project Design**) written in a clear, concise and specific fashion? Are there any ambiguous terms or phrases that need clarification?
- Would the intended audience of your project be able to understand your proposal?
- Have you properly proofread your proposal to assure there are minimal grammatical and spelling mistakes?
- Are all the resources used for this project correctly cited and referenced?
