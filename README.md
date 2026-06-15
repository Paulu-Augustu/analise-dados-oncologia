🏥 Healthcare Analytics: Padrões Oncológicos e Sobrevivência na Índia
Bem-vindo(a) ao repositório do projeto de Healthcare Analytics. Este projeto tem como objetivo demonstrar a aplicação de Análise Exploratória de Dados (EDA) e manipulação de dados em Python num cenário clínico realista.

Através da análise da jornada de pacientes oncológicos — desde o perfil demográfico até ao diagnóstico, tratamento e desfecho clínico —, este dossiê extrai insights valiosos sobre a eficácia das terapias e o impacto do diagnóstico precoce na sobrevivência.

🗄️ Sobre os Dados
O projeto utiliza uma base de dados com 100.000 registos sintéticos de doentes oncológicos na Índia (2022–2025). O dataset foi gerado com base em parâmetros médicos reais e estatísticas populacionais, preservando a privacidade dos doentes, mas mantendo a coerência biológica e clínica ideal para estudos de eficácia e modelos de sobrevivência.

🎯 O que foi analisado? (Principais Insights)
A análise foi dividida em cinco fases cruciais, focadas em responder a perguntas do corpo clínico e da gestão hospitalar:

1. Perfil do Doente (Distribuição Etária)
Objetivo: Descobrir como a idade se relaciona com diferentes tipos de cancro.

Onde ver: Ficheiro GraficoDistrIdadeCancer.png

Insight Clínico: A análise de caixas (Boxplot) revelou que a Leucemia afeta uma população drasticamente mais jovem, enquanto os tumores sólidos (como Próstata e Estômago) têm maior incidência em doentes na faixa dos 60 anos.

2. Mapa Operacional e Tratamentos
Objetivo: Mapear a carga de trabalho do maior hospital da base de dados.

Onde ver: Ficheiro DistrTratamentos.png

Insight Operacional: O Kidwai Memorial Institute of Oncology destacou-se como a instituição com maior volume de atendimentos. A distribuição mostrou que Cirurgias e Cuidados Paliativos representam a maior parte dos procedimentos deste hospital.

3. Validação Clínica e Dinâmica de Género
Objetivo: Cruzar as patologias com o género biológico dos doentes (funcionando como um teste de qualidade de dados).

Onde ver: Ficheiro CancerPorGenero.png

Insight de Integridade: Os dados demonstraram uma fiabilidade clínica de 100%. Cancros exclusivamente femininos (Cervical e Ovário) registaram zero casos em homens, assim como o cancro da Próstata registou zero casos em mulheres.

4. O Fator Crítico: Deteção Precoce
Objetivo: Comprovar matematicamente a relação entre o estádio do cancro no diagnóstico e o tempo médio de sobrevivência.

Onde ver: Ficheiro MediaDeSobr.png

Insight Clínico: O gráfico de linhas comprova a correlação médica: doentes diagnosticados na Fase I (Estádio I) têm uma média de sobrevivência significativamente maior (acima de 24 meses) comparativamente à queda drástica observada na Fase IV (Estádio avançado).

5. Dossiê de Eficácia dos Tratamentos
Objetivo: Calcular a Taxa de Sucesso (%) de cada terapia em relação a cada patologia específica.

Onde ver: Ficheiro relatorio_eficacia_tratamentos.csv

Resultado: Uma tabela executiva pronta a ser consumida por equipas de gestão hospitalar ou dashboards de Business Intelligence, detalhando o volume de doentes, os meses médios de sobrevivência e a taxa percentual de sucesso terapêutico.

📁 Estrutura do Repositório
projeto7.ipynb: O Jupyter Notebook contendo todo o código-fonte, raciocínio analítico, limpeza e visualização dos dados.

*.png: Todos os gráficos exportados durante as análises, prontos a serem integrados em apresentações executivas.

relatorio_eficacia_tratamentos.csv: A base de dados final consolidada (agrupada com a métrica criada de Taxa de Sucesso).

india_cancer_patients_2022_2025.csv: A base de dados sintética original utilizada para o estudo.

🛠️ Tecnologias Utilizadas
Linguagem: Python

Manipulação e Engenharia de Dados: Pandas (Funções de agregação .agg, Criação de Variáveis, Filtros).

Visualização de Dados (Data Viz): Seaborn e Matplotlib (Boxplots, Pie Charts, Lineplots e Countplots).

Ambiente: Jupyter Notebook

*** ### 💡 Como ler este projeto
Se for um recrutador ou gestor de dados, convido-o(a) a abrir o ficheiro .ipynb para analisar a estrutura do código e as boas práticas aplicadas, ou simplesmente a explorar os ficheiros .png para visualizar os resultados da extração de conhecimento clínico.
