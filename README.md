# Otimiza-o-Dashboard-no-Power-BI
Foi pedido para eu otimizar um Dashboard feito no Power BI.

O dashboard estava enfrentando travamentos e não estava atualizando os dados automaticamente. Para abordar esse problema, realizei uma análise detalhada do dashboard usando a ferramenta Measure Killer. Essa ferramenta conduz uma auditoria abrangente, examinando as relações entre colunas, tabelas, medidas, páginas e objetos no dashboard. O resultado dessa análise fornece um relatório detalhado identificando as colunas e medidas que não está sendo utilizada (Imagem 1 e 2).

Com base nas informações obtidas, procedi à remoção de colunas que não estavam sendo utilizadas no dashboard. Contudo, em relação às medidas, optei por não deletar algumas delas. A decisão de manter essa medida está fundamentada na observação de que, embora apresente uma utilização limitada, sua presença não impacta significativamente a performance do dashboard.

É importante notar que essa abordagem foi adotada para otimizar o desempenho geral, concentrando-me na remoção de elementos desnecessários. A medida preservada, mesmo com sua baixa relevância, não demonstrou influenciar negativamente a eficiência do dashboard, e sua retenção contribui para uma compreensão mais completa do modelo de dados.

Assim, busquei um equilíbrio entre a otimização da performance e a preservação de elementos que, apesar de sua baixa utilização, não apresentavam impacto significativo. Essa abordagem visa assegurar que o dashboard permaneça ágil e eficiente, mantendo a integridade das informações apresentadas.

<p align="center">
  <img src="https://github.com/FabricioPP/Otimiza-o-Dashboard-no-Power-BI/assets/18078359/3040ad11-be49-47e5-9345-1cc5ec0c7b3e" alt="Grafico contagem de colunas usadas e nao usadas" width="500">
  <br>
  <em>Imagem 1: Gráfico de colunas usadas e não usadas no Dashboard.</em>
</p>

<p align="center">
  <img src="https://github.com/FabricioPP/Otimiza-o-Dashboard-no-Power-BI/assets/18078359/abc53611-9341-4963-b645-f88d51423af2" alt="Grafico das tabelas do dashboard e as colunas usadas e nao usadas" width="800">
  <br>
  <em>Imagem 2: Gráfico das tabelas do Dashboard com a contagem de colunas usadas e não usadas.</em>
</p>

<p align="center">
  <img src="https://github.com/FabricioPP/Otimiza-o-Dashboard-no-Power-BI/assets/18078359/73b577bf-aae0-4045-9d98-e2805ee7d70a" alt="Grafico do tamanho de cada tabela em MB" width="500">
  <br>
  <em>Imagem 3: Tabelas com seus respectivos tamanhos em MB de colunas não usadas.</em>
</p>

Após exclusões o número diminuiu de 201 para 76 (Imagem 4 e 5), resultando em uma diminuição de aproximadamente 400MB no dashboard (Imagem 4), com uma notável otimização no desempenho do dashboard.

<p align="center">
  <img src="https://github.com/FabricioPP/Otimiza-o-Dashboard-no-Power-BI/assets/18078359/acc690f3-2beb-42a6-a5f8-7dd901bc9e9e" alt="Grafico apos exclusoes" width="500">
  <br>
  <em>Imagem 4: Gráfico após exclusões.</em>
</p>

<p align="center">
  <img src="https://github.com/FabricioPP/Otimiza-o-Dashboard-no-Power-BI/assets/18078359/87ab83f4-742f-4d93-8780-707e1b072c36" alt="Grafico das tabela apos exclusoes" width="800">
  <br>
  <em>Imagem 5: Gráfico das tabelas do Dashboard com a contagem de colunas usadas e não usadas após exclusões.</em>
</p>

<p align="center">
  <img src="https://github.com/FabricioPP/Otimiza-o-Dashboard-no-Power-BI/assets/18078359/87f3708e-a0e0-4eda-b7ea-a1e21e4184d9" alt="Grafico tamanho em MB de cada Tabela" width="500">
  <br>
  <em>Imagem 6: Tabela com seus respectivos tamanhos (após exclusões) em MB de colunas não usadas.</em>
</p>

Fiz uma otimização da consulta SQL também, mas por questões éticas não posso compartilhar as mudanças, por ser uma consulta que pode haver informações confidencias. Mas no resumo
deletei algumas colunas que estavam sendo trazidas juntas sem a necessidade, eliminei algumas redundâncias e otimizei os parâmetros de acordo com o solicitado.
