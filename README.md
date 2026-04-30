SVDC - Exercício

UTILIZEI O CSV DO COVID, NAO CONSIGO DAR UPLOAD POR CAUSA DO TAMANHO
Os meus principais objetivos com este dataset são:

- Analisar a eficácia das medidas de restrição (confinamentos/lockdowns) em relação ao surgimento de novos casos.
- Mapear a propagação global do vírus, ajustada à proporção populacional de cada país.
- Acompanhar a "Corrida das Vacinas", comparando a velocidade e o sucesso das campanhas de vacinação entre nações.
- Identificar padrões de reporte de dados utilizando mapas de calor temporais (sazonalidade e dias da semana).
  
Primeiramente, estudamos o impacto das regras de contingência nos novos casos. Diferentes países tiveram diferentes níveis de contingência, e podemos analisar se as restrições (ficar em casa, distanciamento social, etc.) afetaram a quantidade de casos. O objetivo é ver se um aumento no nível de contingência levou, posteriormente, a uma diminuição de novos casos e por isso usamos Dual Axis onde temos nas Rows Stringency Index e New cases. 

No Heatmap, tentamos perceber em que dia da semana há mais relatos de casos. No caso de Portugal, por exemplo, nota-se um pico ao domingo. Podemos assumir então que, numa certa fase, Portugal apenas atualizava os dados dos novos casos uma vez por semana (ao domingo). Usamos filtro de país para ver apenas Portugal ou outro país e temos semana como coluna e weekday como row para conseguirmos ver por dia da semana por fim temos new cases como Color Marks.

Temos outro gráfico onde comparamos a velocidade a que a vacina foi administrada à população. Podemos reparar que, em países de baixo rendimento (Lower Income Countries), a velocidade de vacinação foi muito inferior em relação à de países com mais recursos. Portugal teve um bom desempenho neste aspeto, alcançando até uma percentagem de vacinação superior à de países como a Alemanha. Para este cálculo vamos analisar a percentagem de população vacinada ao longo do tempo criando uma calculated field.

Através do mapa, podemos observar a percentagem da população infetada, sendo visível que, em Portugal, mais de metade da população já teve COVID-19. Para este cálculo divido a população infetada pela população máxima.

Em todos estes gráficos temos a opção de filtrar e analisar outros países para além de Portugal.
Adicionei também 2 banners (KPIs): um de Casos Totais e outro de Mortes Totais. Para estes, criei Calculated Fields onde somei o número máximo de casos e mortes de cada país.
Outros Calculated Fields que criei foram a Percentagem Infetada e a Percentagem Vacinada. Estes valores foram calculados dividindo o número de pessoas totalmente vacinadas (ou infetadas) pela população total do país.

https://public.tableau.com/app/profile/nuno.ni/viz/Book3_17775609382690/Dashboard1?publish=yes

RESULTADOS: 
<img width="2159" height="1289" alt="image" src="https://github.com/user-attachments/assets/525f656b-c5e8-49cc-8412-c6c3c4f7c4a3" />
<img width="2159" height="1288" alt="image" src="https://github.com/user-attachments/assets/79c9d37d-f5cb-404e-a517-ea1ddbc2d5db" />
<img width="2158" height="1179" alt="image" src="https://github.com/user-attachments/assets/d6657f3b-3f61-4306-a2d1-9de5f835897b" />
<img width="2159" height="1301" alt="image" src="https://github.com/user-attachments/assets/5e2f26fd-cddb-446d-b739-99f94d3b66ba" />
<img width="2159" height="1288" alt="image" src="https://github.com/user-attachments/assets/e0fd6d44-645e-4e23-8760-15a219c764db" />
