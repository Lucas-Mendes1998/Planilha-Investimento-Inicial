# DIO INVEST — Simulador de Investimentos

## Sobre o projeto

A DIO INVEST é uma ferramenta desenvolvida em Excel para simular a evolução do patrimônio por meio de aportes mensais, estimar possíveis rendimentos e auxiliar na distribuição de investimentos em Fundos de Investimento Imobiliário (FIIs), conforme o perfil selecionado.

## Funcionalidades

- Simulação de patrimônio acumulado com diferentes prazos de investimento.
- Projeções para 2, 5, 10, 20 e 30 anos.
- Estimativa de dividendos mensais.
- Sugestão de investimento equivalente a 30% do salário informado.
- Distribuição de aportes entre seis categorias de FIIs.
- Seleção entre os perfis Conservador, Moderado e Agressivo.

## Fórmulas utilizadas

### VF — Valor Futuro

A função `VF` calcula o patrimônio futuro a partir de aportes periódicos, taxa de rendimento mensal e prazo de investimento.

### PROCV — Busca de percentuais

A função `PROCV` identifica o percentual de alocação correspondente ao perfil e à categoria de FII selecionados, consultando a tabela de parâmetros da segunda aba.

Os valores de cada categoria são calculados multiplicando o percentual encontrado pelo aporte mensal destinado à distribuição.

## Estrutura da planilha

- **Planilha1:** interface principal, configurações, simulações, dividendos e distribuição dos aportes.
- **Planilha2:** tabela de percentuais por perfil e categoria de FII.

## Intervalos nomeados

A ferramenta utiliza os intervalos `aporte`, `patrimonio`, `qtd_anos`, `Rendimento_carteira`, `salario`, `sugestao_investimento` e `taxa_mensal` para facilitar a leitura e a manutenção das fórmulas.

## Perfis de alocação

Os percentuais são configurados na segunda aba da planilha:

- **Conservador:** Papel 30%, Tijolo 50%, Híbridos 10%, FOFs 10%, Desenvolvimento 0% e Hotelarias 0%.
- **Moderado:** Papel 32%, Tijolo 40%, Híbridos 8%, FOFs 10%, Desenvolvimento 5% e Hotelarias 5%.
- **Agressivo:** Papel 50%, Tijolo 10%, Híbridos 5%, FOFs 5%, Desenvolvimento 20% e Hotelarias 10%.

Os percentuais são parâmetros internos da ferramenta. Sua fonte metodológica não está documentada no arquivo analisado.

## Limitações

Os resultados são projeções matemáticas baseadas nos parâmetros informados. Rentabilidade, dividendos e patrimônio futuro não são garantidos. A ferramenta não substitui uma análise individualizada de risco e adequação dos investimentos.

## Tecnologias e recursos

- Microsoft Excel
- Fórmulas financeiras (`VF`)
- Busca de dados (`PROCV`)
- Intervalos nomeados
- Tabelas de parâmetros e simulações
