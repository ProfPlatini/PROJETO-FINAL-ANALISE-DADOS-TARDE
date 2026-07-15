## Projeto de Machine Learning para previsão de valores de carros

Projeto desenvolvido durante o curso de Fundamentos de I.A. e Análise de Dados 

---
### Tecnologias utilizadas:
- Python
- Bibliotecas: Pandas, Scikit-Learn, Numpy, Seaborn
- Frameworks: Flask e CORS
- Deploy e CD: Render
- FrontEnd: Lovable 
---
### Como funciona? 
O modelo utiliza a base de dados ```dataset_carros_usados.csv``` para realizar previsões e estimar o preço de um veículo de acordo com algumas informações específicas: 
- Ano de fabricação
- Quilometragem 
- Motor 
- Quantidade de revisões 
---
### Arquitetura
O modelo de M.L. está hospedado no Render.com, funcionando como uma API, retornando o preço estimado no formato JSON quando realizada uma requisição do tipo *POST* para o link:

https://projeto-final-analise-dados-tarde.onrender.com/prever 

*Obs*: Para testes iniciais, realizar uma requisição do tipo GET para o link:

https://projeto-final-analise-dados-tarde.onrender.com
---
### Links

- Site publicado: https://wheel-price-predictor.lovable.app/
- API (Modelo de Machine Learning): https://projeto-final-analise-dados-tarde.onrender.com 
