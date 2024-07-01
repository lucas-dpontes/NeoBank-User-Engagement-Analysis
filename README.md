# le-wagon-final-project



This is a course completion project of a 400-hour training bootcamp in Data Analytics, at Le Wagon Programming School.

Technologies and methods used:
- Python libraries (Google Collaboratory)
- SQL (Google BigQuery)
- Data Visualization (Looker Studio)
- Statistical tests (Chi-square)

This project aimed to study churners at Neo Bank, a digital bank that offers a range of services and financial products with the difference that customers do not need to worry about hidden fees.

```mermaid
flowchart LR
    id1(40M +

Personal account customers
) ~~~     id2(500k +

Commercial account customers
)
```

SITUATION

One of the main pain points was the lack of visibility into churners, who are customers who abandoned the service.

TASK

Based on this scenario, our project aimed to meet 3 main objectives:

1. Raise hypotheses guiding the project and validate them through statistical methods

2. Find a definition of churner that makes sense for the business needs, considering the available data

3. Extract actionable insights that help to better understand this evasion and propose improvement actions

Our time frame was from January to October 2018, that is, this was the period chosen to conduct this study.

Therefore, the project was developed considering a churner as a user who has had an account for at least 6 months and who has not made a transaction for 6 months or more

```mermaid
---
title: Churner
---
flowchart LR
    id1(Existing users for more than 6 months whose last
transaction occurred at least 6 months ago
)
```

Portanto, o projeto foi desenvolvido considerando churner como um usuário que tem conta há pelo menos 6 meses e que está há 6 meses ou mais sem fazer uma transação

ACTIONS

```mermaid
---
title: ETL process
---
flowchart LR
    A["Cleaning the
raw data"] --> B["Exploratory analysis
of clean data"] --> C["Definition and validation 
of hypotheses"] --> D["Statistical
analysis"]
```

```mermaid
---
title: Dataset
---
flowchart LR
    id1[(users)] ~~~ id2[(transactions)] ~~~ id3[(notifications)] ~~~ id4[(devices)]
```

The flowchart above, known as ETL that means to extract, transform and load, representa as principais atividades executadas, sendo que precisamos dar bastante atenção à limpeza e análise dos dados. Optamos por fazer validação de hipóteses assim como análises estatísticas para tirar insights valiosos das nossas análises, buscando seguir a metodologia científica.

RESULTS

Levando em conta o recorte temporal do ano de 2018, há mais de 13 mil usuários ativos, sendo que desses 18,7% são churners.

Nós constatamos que há relação entre a idade e a taxa de churn, com a geração Baby Boomer (ou seja, aqueles que nasceram até 1965) e o início da geração X (nascidos entre 65 e 87) sendo os maiores churners

E os Millennials (nascidos entre 88 e 96) com os menores valores. Apesar disso não ser compatível com o movimento global, isso pode ser explicado pelo recorte temporal utilizado e o fato dos Millenials e Gen Z terem uma tendência maior a fazer o que é chamado de churn e return, que é a evasão do produto e uma possível volta caso exista necessidade ou quando os benefícios voltam a ser vantajosos.

Fazendo uso dessa divisão em gerações, podemos ver o impacto do uso de criptomoedas para todas as idades. Quando um usuário habilita a possibilidade de investir em criptomoedas, isso reduz muito a possibilidade de se tornar churner, 

tendo o maior impacto na geração Z, com a queda de 22,5% para 4,5%. A queda da taxa de churn é maior nos usuários mais novos, talvez pela facilidade com as novas tecnologias, mas o impacto é visível nos quatro grupos.

Outro ponto que chamou a nossa atenção foi que clientes do plano gratuito (STANDARD) possuem uma taxa de churn muito maior que dos planos pagos, que são o PREMIUM e o METAL. 

O plano METAL, inclusive, teve uma taxa de churn de 0% e o plano PREMIUM de apenas 1,67%. Uma diferença enorme pro plano STANDARD com 20%.

Também constatamos uma relação entre o número de contatos e a taxa de churn. Quanto mais conectado com outros usuários, menores são as chances de um cliente parar de utilizar o produto. 

Um usuário com 0 contatos tem um churn rate de 32%, bem acima da média de referência de quase 19%, e esse número vai caindo quanto mais contatos um usuário possui.

Isso também é constatado pela análise dos usuários por países, onde é possível ver que a taxa de churn costuma ser menor nos países com uma média de contatos por usuário maior. 

Aqui temos a nossa taxa média de churn e é possível ver como países com mais contatos por usuário estão consideravelmente abaixo desse número, com a Romênia com 9,4% e a Irlanda com 10,5%, por exemplo. 

Seguindo o gráfico, vemos que os clientes de países com mais de 20% de taxa de churn são os que menos têm contatos por usuário.

Por fim, vimos que usuários com dispositivo Apple tendem a fazer mais churn. É possível que exista uma relação com erros nos aplicativos, considerando que existiram alguns picos de falhas de envio de notificações para usuários ao longo dos meses.

O mês de março foi o mês de maior erros no envio de notificações e também o mês com o maior número de churn no período (332 usuários).
O mês de outubro, em contrapartida, foi o mês com o maior número de notificações enviadas com sucesso e foi o mês com o segundo menor número de churn, com 191 usuários, atrás apenas do mês de fevereiro (172 usuários).

CONSIDERAÇÕES FINAIS
Com base nos insights extraídos e nas análises do negócio, gostaríamos de propor o desenvolvimento de planos de ação para atender esses 4 direcionadores:

Reter e engajar que os usuários invistam nas criptomoedas. Observamos que usuários que investem em criptomoedas tem uma taxa de churn menor do que aqueles que não investem. E olhando mais a fundo, dividindo esses usuários em faixa etária, observamos que quanto mais jovem menor o churn. Dessa forma a sugestão é não apenas ter um investimento maior nos investidores de cripto mas também focar nos usuários mais jovens;
Oferecer mais benefícios e promoções para o plano gratuito, que possui um churn rate e quantidade de usuários muito maior em relação aos pagos, que tem uma representatividade bem menor de usuários;
Encorajar usuários a terem mais contatos salvos no app por meio de promoções e notificações. Isso porque usuários com 1 ou nenhum contato têm, respectivamente, um churn de aproximadamente 23 e 33%, enquanto que usuários com 10 ou mais contatos tem um churn médio de 6.5%;
Melhorar a experiência dos usuários nos aplicativos, especialmente no sistema iOS, que tem um percentual maior de churn comparado aos usuários que têm o sistema Android.
