# Tratamento-de-Dados-de-forma-Pratica-utilizando-a-linguagem-Python
Este projeto foi uma oportunidade de trabalhar um pouco mais a fundo com um dataset simples sobre clima, usando Python para explorar, visualizar e tratar os dados. Apesar de ser um conjunto pequeno, ele trouxe vários pontos interessantes para praticar análise exploratória e limpeza — algo que, na vida real, faz toda a diferença antes de qualquer modelagem.

Logo no início, importei três bibliotecas que deram conta de todo o fluxo: Pandas, para manipular os dados; Seaborn, para os gráficos; e Statistics, para cálculos como mediana. Depois de carregar a base com read_csv, dei uma olhada nas primeiras linhas para entender o formato geral e já identificar possíveis problemas.

Comecei observando as variáveis categóricas. Agrupei os dados por Aparência, Vento e Jogar, e criei gráficos de barras para visualizar a distribuição desses valores. Foi uma forma rápida de perceber padrões e também possíveis inconsistências nos dados.

Em seguida, foquei nas variáveis numéricas: Temperatura e Umidade. Usei estatísticas descritivas para entender a faixa de valores, e complementei com boxplots e histogramas para detectar outliers e analisar a distribuição. Esses gráficos mostraram que a coluna de Umidade tinha valores fora do intervalo real (abaixo de 0% ou acima de 100%), além de alguns valores nulos.

Para tratar isso, calculei a mediana da Umidade e utilizei esse valor tanto para preencher os dados faltantes quanto para substituir valores inválidos. Dessa forma, mantive a integridade da distribuição sem distorcer demais seus valores. Já a coluna Vento apresentava alguns valores nulos, que também foram preenchidos — desta vez com o valor "FALSO", mantendo consistência com o restante da base.

Depois desses ajustes, revisei novamente as colunas para confirmar que não haviam sobrado valores nulos nem pontos fora dos limites aceitáveis. O dataset final ficou mais limpo, coerente e pronto para ser utilizado em outras análises, visualizações ou até para servir de base para um modelo simples no futuro.

Esse projeto reforça algo que considero essencial: mesmo datasets pequenos podem esconder desafios reais — e trabalhar o básico com calma faz toda a diferença. Além disso, foi uma ótima oportunidade para praticar visualização e tratamento de dados utilizando o ecossistema Python.
