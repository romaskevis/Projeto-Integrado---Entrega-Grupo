# Números que Falam — síntese do grupo
**Consultoria de dados públicos · Python e Matemática · 06/11/2026**

## Objetivo e execução
Transformar exportações oficiais do IBGE em análises territoriais para gestores públicos. O painel integra quatro indicadores e abre com bases locais. O módulo individual de Bernardo Romaskevis é Crescimento demográfico, conforme a entrega anterior. A identificação dos demais integrantes e o quinto módulo exigido pelo guia permanecem pendentes.

## Principais achados
**Crescimento:** a média simples entre 5.570 unidades municipais foi 3.65% entre 2010 e 2022, contra mediana de 1.60%. A regra 1,5 IQR sinalizou 279 extremos. Prefeituras devem adaptar o planejamento à direção e intensidade da mudança, investigando as causas antes de decidir investimentos.

**Trabalho:** entre UFs, a maior redução da taxa total ocorreu em Roraima, com -2.70 pontos percentuais. Isso não responde qual UF mais reduziu o número absoluto de desempregados: a base só traz taxas. No Brasil, a taxa total passou de 7,3% para 9,5%, diferença de 2,2 pontos percentuais. Governo e setor produtivo podem priorizar investigação dos territórios e desigualdades por sexo, mas os dados não medem formalidade nem paridade salarial.

**Afazeres:** a diferença média simples entre taxas estaduais de horas de mulheres e homens em 2022 foi 9.37 horas; a maior foi em Sergipe (13.50 horas). Para as personas, recomenda-se investigar demanda por creches e serviços de cuidado. Não é possível separar raça ou ocupação nessa exportação, nem testar significância com médias sem erros amostrais.

**Superior:** a proporção de pessoas de 25 anos ou mais com superior completo em 2022 variou de 11.34% em Maranhão a 36.90% em Distrito Federal. O painel apresenta a evolução disponível por UF. A razão não é taxa de diplomação de ingressantes; não há suporte para comparar cursos de Exatas/Humanas ou mulheres em STEM.

## Método e rigor
ETL em Pandas; CSV em formato longo; preservação dos XLSX e notas; validação de unidades; filtros por território, região, ano e sexo quando disponível. Média, mediana, moda, quartis, IQR, amplitude, variância e desvio populacional e outliers são recalculados para um nível e uma medida por vez. Não se misturam totais nacionais com suas subdivisões. Outliers são mantidos e explicitados. Valores ausentes não são convertidos em zero.

## Entrega e cobertura
Código Python, quatro bases originais, CSVs tratados, painel Streamlit, testes, análise individual e instruções de execução acompanham esta síntese. Os recortes ausentes e o quinto módulo estão listados em COBERTURA.md. A apresentação oral precisa ser estudada e realizada pelos integrantes.

Fontes: SIDRA/IBGE, tabelas [4709](https://sidra.ibge.gov.br/tabela/4709), [9694](https://sidra.ibge.gov.br/tabela/9694), [7015](https://sidra.ibge.gov.br/tabela/7015) e [7135](https://sidra.ibge.gov.br/tabela/7135), arquivos fornecidos em 06/11/2026.
