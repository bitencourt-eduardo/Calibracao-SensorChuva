# Desafio Técnico de Dados da FieldPRO

<h1 align="center"> <img src="https://fieldpro.com.br/wp-content/themes/fieldpro/src/images/logo.png" width=180px></h1>   

<h2>Status do Projeto</h2>

![Badge Status](http://img.shields.io/static/v1?label=STATUS&message=EM%20REVISÃO&color=GREEN&style=for-the-badge)


# Índice
<!--ts-->
   * [Objetivo](#objetivo)
   * [Requisitos](#requisitos)
   * [Dados](#dados)
   * [Ferramentas e Tecnologias](#ferramentas-e-tecnologias)
   * [Conclusão](#conclusao)
 
<!--te-->
 
 # 🧾 Objetivo

O objetivo deste desafio é construir um modelo de calibração de um sensor de chuva baseado em impactos mecânicos. O sistema de medição de chuva funciona por meio de uma placa eletrônica com um piezoelétrico, um acumulador de carga e um sensor de temperatura. Os dados são transmitidos de hora em hora. É importante considerar que o impacto das gotas de chuva gera vibrações no piezoelétrico, induzindo uma corrente elétrica, que é acumulada ao longo do tempo e gera uma queda na carga do acumulador.

O número de resets da placa também pode afetar o comportamento do acumulador de carga, portanto, pode ser relevante incluir essa informação no modelo.
 
# Requisitos


<img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" width="80" height="80"/><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/c/c3/Python-logo-notext.svg/935px-Python-logo-notext.svg.png" width="70" height="70"/><img src="https://jupyter.org/assets/homepage/main-logo.svg" width="80" height="80"/> 

- [x] Crie um repositório público no GitHub para o desafio técnico;
- [x] Faça o upload de todo o código-fonte e qualquer arquivo adicional necessário para executar o projeto:
   
Notebook Jupyter que conterá as 
- [x]  Análises preliminares e visualizações, 
- [x] Pipeline de transformação de dados
- [x] Treinamento do(s) modelo(s)
- [x] Análises de performance

Opcionalmente:
- [x] forneça um arquivo README.md no repositório contendo quaisquer considerações adicionais que você julgar relevante.

# Dados

Os arquivos de dados `Sensor_FieldPRO.csv` e `Estacao_Convencional.csv` estão disponíveis para a análise.

### Variáveis do arquivo Sensor_FieldPRO.csv

As medidas realizadas pelo sensor incluem:

- `piezo_charge`: Carga medida no acumulador.
- `piezo_temperature`: Temperatura da placa.
- `num_of_resets`: Número total de resets da placa desde que foi ligada pela primeira vez.
- `air_temperature_100`: Temperatura do ar externo.
- `air_humidity_100`: Umidade relativa do ar externo.
- `atm_pressure_main`: Pressão atmosférica.
- `Datetime – utc`: Date e hora em pradão ISO-8601.


### Variáveis do arquivo Estacao_Convencional.csv

As medidas realizadas pelo sensor incluem:

- `Data`: Data de transmissão.
- `Hora (Brasília)`: Hora de transmissão.
- `chuva`: Esta é a variável alvo que queremos prever..


# Estrutura do Projeto
- code	_(pasta com os notebooks desenvolvidos)_
  - 01_trantamento.ipynb
  - 02_analise_exploratória.ipynb
  - 03_normalizacao.ipynb
  - 04_Balanciamento.ipynb
  - 05_Modelagem.ipynb
- datasets  _(pasta com os arquivos CSV necessários)_
    - Estacao_Convencial.csv      
    - Sensor_FielPRO.csv
    - ..
- README.md
- desafio.pdf

O códigos notebook estão devidamente comentados para explicar cada etapa da solução abordada.


# 🛠Ferramentas e Tecnologias

<table>
<tr>
	<th>Dependência</th>
	<th>Versão</th>
</tr>
<tr>
	<td>Python</td>
	<td>3.11</td>
</tr>
<tr>
	<td>Jupyter</td>
	<td>6.4.12</td>
</tr>	
<tr>
	<td>Pandas</td>
	<td>2.0.4</td>
</tr>	
<tr>
	<td>Matplotlib</td>
	<td>3.7.2</td>
</tr>
<tr>
	<td>Seaborn</td>
	<td>0.12.0</td>
</tr>
<tr>
	<td>scikit-learn</td>
	<td>1.3.0</td>
</tr>
<tr>
	<td>imbalanced-learn</td>
	<td>0.11.0</td>
</tr>
<tr>
	<td>xgboost</td>
	<td>1.7.6</td>
</tr>
</table>


# Considerações Adicionais

Fiz uso da biblioteca pandas para carregar e manipular os dados dos arquivos CSV.
Utilizei scikit-learn para criar o pipeline de transformação de dados e treinar o(s) modelo(s) necessário(s).
Incluí visualizações e análises preliminares para melhor compreensão dos dados.
Os códigos estão divididos em estapas para sequênciais numeradas e está devidamente comentado para explicar cada etapa da solução abordada.

Sinta-se à vontade para entrar em contato caso tenha alguma dúvida ou sugestão de melhoria.



# Considerações para análises futuras

- Realizar conjunto de testes para diferentes condições
   -  Elevadas altitudes
   - Condições +40 ºC e - 0ºC
- Verificar interferência de forças do vento sobre as medidas
 
<h2>Desenvolvedo por:  </h2>
<div>

![Linkedin Badge](https://img.shields.io/badge/-Eduardo_Bitencourt-blue?style=flat-square&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/bitencourt-eduardo/)
![GitHub Org's stars](https://img.shields.io/github/stars/bitencourt-eduardo?style=social)
</div> 

