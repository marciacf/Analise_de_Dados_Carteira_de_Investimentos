# Redução do Risco pela Diversificação da Carteira de Investimentos
## Projeto de Análise de Dados visando a utilização de técnicas para a redução do risco de uma carteira de investimentos

Existem diversas possibilidades de aplicações financeiras disponíveis no mercado. Ao realizar um investimento é preciso avaliar o risco e o retorno. Geralmente, investimentos de maior risco geram melhores retornos financeiros e investimentos de menor risco geram retornos menores. Para diminuir o risco de um investimento algumas ferramentas e técnicas podem ser adotadas.

A diversificação de investimentos é uma estratégia muito aplicada para reduzir os riscos no aporte de recursos. Visando setores diferentes, ativos distintos e mercados variados.

Este trabalho mostra como o risco de um investimento pode ser reduzido por meio da diversificação da carteira.
Foi considerado uma carteira de ações de 9 empresas que um investidor possui. São elas: Arezzo, B3, Klabin, Localiza, Multiplan, Petrobras, Rede Atacadão, SulAmerica e Vale.

Abaixo temos a variação do preço dos Ativos ao longo do período de agosto de 2019 a julho de 2021. 

![Captura de tela 2024-06-03 121916](https://github.com/marciacf/Analise_de_Dados_Projeto_Turnover/assets/102993177/de7ed5b5-4d57-47da-a549-90d13a5ed7b9)

### Mostrando como a diversificação de investimentos é importante:

###  -   Correlação entre os Ativos

Investir em ativos que sejam pouco relacionados entre si, diminui o risco da carteira de investimentos. Essa ação contribui para proteger a carteira contra oscilações do mercado financeiro, assim, quando um ativo perde, o outro ativo pode ganhar ou continuar constante. 

É importante avaliar a correlação entre os ativos, para que um investidor não coloque todo o seu dinheiro em apenas um tipo de investimento (famoso “colocar todos os ovos na mesma cesta’’)
Se os ativos forem muito correlacionados, perde-se o efeito da “diversificação”.

Desta forma, foi analisada a correlação entre os ativos usando correlação de Pearson e não há nenhuma correlação forte entre as empresas.

Correlação de Pearson dos Ativos:

![Captura de tela 2024-06-03 122556](https://github.com/marciacf/Analise_de_Dados_Projeto_Turnover/assets/102993177/ba500aa5-e4c0-4d6f-a007-5d04d48fc276)

 ###  -  Cálculo do risco
 
O cálculo de risco é fundamental para uma carteira de investimentos, pois permite ao investidor avaliar e gerenciar os possíveis perigos associados aos ativos, ajudando a equilibrar o potencial de retorno com a exposição ao risco.

O cálculo de risco é o desvio padrão dos retornos. O desvio padrão é uma medida estatística que quantifica a dispersão dos retornos de um investimento em relação à média. Um desvio padrão maior indica maior volatilidade e, portanto, maior risco.

O retorno de um ativo é a variação percentual do preço do dia anterior para o dia atual. Ou seja, Retorno Hoje = (Preço hoje – Preço Ontem) / Preço Ontem.

![Captura de tela 2024-06-03 123029](https://github.com/marciacf/Analise_de_Dados_Projeto_Turnover/assets/102993177/bea0a8d4-0a8b-421f-ae05-6a02108f1f8d)

O desvio padrão da carteira é menor que o desvio padrão de cada um dos investimentos separados. Mostrando o benefício estatístico da diversificação.  

Portanto, o risco de uma carteira diversificada é menor do que investir em um único ativo. Assim, o investidor tem uma carteira menos arriscada.

 ### - Cálculo do VaR
 
Um dos métodos adotados para o gerenciamento desse tipo de risco é o cálculo do VaR (Value at Risk). O Var é um indicador de risco que considera a perda máxima possível de um investimento em um período de tempo.

Essa metodologia utiliza algumas técnicas estatísticas para o cálculo da maior perda esperada de um título (Ação) ou carteira de títulos (Ações) em condições normais de mercado e supondo que o risco futuro permaneça de maneira semelhante ao que já ocorreu no passado.

Usando os dados resultantes da modelagem do VaR, a instituição financeira pode decidir se tem reservas de capital suficientes para cobrir perdas ou se os riscos acima do aceitável exigem mudanças na carteira para investimentos de menor risco.

Para o cálculo do VaR foi usada uma base histórica diária de preços dos ativos.
Foi considerado um saldo de valor investido na carteira pelo investidor de R$ 1.000.000,00 reais (um milhão de reais).

Distribuição do valor investido por ação:

![Captura de tela 2024-06-03 123309](https://github.com/marciacf/Analise_de_Dados_Projeto_Turnover/assets/102993177/c5015f51-2ef0-4956-a66f-b82faf3113f0)

Foi calculado o valor de retorno que equivale ao percentil 5% dos retornos diários. Esse valor é multiplicado pela quantidade em reais que se tem de cada ativo em reais. 
O horizonte de tempo adotado para o cálculo do VaR foi dos últimos 180 dias.

![Captura de tela 2024-06-03 141825](https://github.com/marciacf/Analise_de_Dados_Projeto_Turnover/assets/102993177/7c0466cf-5c25-4668-a517-082a794f0d0f)

O VaR mostra que existe 5% de probabilidade de a carteira ter uma perda (desvalorização) maior que R$18.420,31 reais em um dado horizonte de tempo (180 dias).

O VaR da carteira do investidor (R$ 18.420,31) é menor que a soma dos VaR’s individuais (R$ 29.456,11)
Mais uma vez mostrando que o risco da carteira é menor que o risco dos ativos individuais.

### Considerações finais:

O entendimento do conceito de risco e retorno no mundo das finanças envolve analisar as possíveis dificuldades que um investimento pode apresentar, ao mesmo tempo em que se mede os retornos esperados.

O equilíbrio entre risco e retorno é fundamental para uma carteira saudável e bem-sucedida.

Investir em uma carteira diversificada, com ações de empresas e setores não correlacionados é uma estratégia para diminuição de riscos.

Vale ressaltar que o mercado financeiro é um ambiente complexo e dinâmico. O preço dos ativos financeiros pode variar em curtos períodos de tempo. Essa volatilidade é influenciada por fatores econômicos, políticos e até mesmo eventos como pandemia e desastres naturais. 

A incerteza e o risco fazem parte do mercado financeiro, mas com estratégias bem fundamentadas, os investidores podem tomar decisões financeiras inteligentes e construir uma estratégia de investimento sólida.



