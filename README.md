# Calibracao-SensorChuva

# Desafio Técnico de Dados da FieldPRO

Bem-vindo ao desafio técnico de dados da FieldPRO!

<h1 align="center"> <img src="https://fieldpro.com.br/wp-content/themes/fieldpro/src/images/logo.png" width=180px></h1>   

<h2>Status do Projeto</h2>

![Badge Status](http://img.shields.io/static/v1?label=STATUS&message=EM%20REVISÃO&color=GREEN&style=for-the-badge)


# Índice
<!--ts-->
   * [Sobre](#sobre)
   * [Requisitos](#requisitos)
   * [Estruturação de Dados](#estruturação-de-dados)
   * [Ferramentas e Tecnologias](#ferramentas-e-tecnologias)
 
<!--te-->
 
 # 🧾 Objetivo

O objetivo deste desafio é construir um modelo de calibração de um sensor de chuva baseado em impactos mecânicos. O sistema de medição de chuva funciona por meio de uma placa eletrônica com um piezoelétrico, um acumulador de carga e um sensor de temperatura. Os dados são transmitidos de hora em hora.

 
## Modelagem

A tarefa é construir um modelo de calibração para o sensor de chuva com base nas informações disponíveis. É importante considerar que o impacto das gotas de chuva gera vibrações no piezoelétrico, induzindo uma corrente elétrica, que é acumulada ao longo do tempo e gera uma queda na carga do acumulador.

O número de resets da placa também pode afetar o comportamento do acumulador de carga, portanto, pode ser relevante incluir essa informação no modelo.


## Arquivos de Dados

Os arquivos de dados `Sensor_FieldPRO.csv` e `Estacao_Convencional.csv` estão disponíveis para a análise.

## Descrição dos Dados

Os dados disponíveis para este desafio estão no arquivo `Sensor_FieldPRO.csv`. Além disso, foram utilizadas medidas de uma estação meteorológica próxima, disponíveis no arquivo `Estacao_Convencional.csv`. Ambos estão armazenados na pasta _datasets_

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


## Instruções de Execução

Para executar o código relacionado ao desafio, siga as instruções abaixo:

1. Clone este repositório para sua máquina local.
2. Certifique-se de ter as dependências e bibliotecas necessárias instaladas.
3. Execute o script de calibração e análise de dados.
4. Analise os resultados e ajuste o modelo conforme necessário.

## Conclusão

Este é um desafio empolgante de calibração de um sensor de chuva. Lembre-se de documentar suas decisões e abordagens ao longo do processo de modelagem. Boa sorte e divirta-se!

**Nota:** Para informações adicionais sobre os dados e o desafio, consulte o conteúdo completo do documento fornecido.

Se houver alguma dúvida ou precisar de mais informações, sinta-se à vontade para entrar em contato.

*Esse é apenas um exemplo de arquivo README em formato Markdown. Lembre-se de adaptar o conteúdo conforme necessário para o seu projeto ou desafio específico.*

 Desenvolvimento de API de simulação de banco, com operações bancárias do dia a dia, obedencendo algumas entregas mínimas como:
  
  
- [x] Cadastro de Clientes<br>
- [x] Buscar os Clientes Cadastrados<br>
- [x] Transferências de saldo entre as contas<br>
- [x] Buscar o histórico de transações entre as contas<br>

# Requisitos 

<img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" width="80" height="80"/><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/c/c3/Python-logo-notext.svg/935px-Python-logo-notext.svg.png" width="70" height="70"/><img src="https://jupyter.org/assets/homepage/main-logo.svg" width="80" height="80"/> 

* Ter instalado na sua máquina: MySQL, uma IDE (recomendamos o Intellij) e Java.
* Como rodar a aplicação: Clone este repositório
* Configure o arquivo application.properties com seu dados pessoais do Banco de dados de MySql: o SQL para popular o banco de dados no MySQL Workbench se encontra na pasta `bancoDeDados` e o arquivo é chamado de `bd_divasbank.sql`.
* Caso prefira utilizar o banco de dados H2, o projeto já possui esta dependência.
* Acesse a pasta do projeto no terminal/cmd e vá para a pasta do Divas Bank,
* Execute a aplicação: o servidor entra pela porta 8080.

# Estrutura do Projeto





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
	<td>Matplotlib</td>
	<td>3.7.2</td>
</tr>
</table>


# Considerações Adicionais

Fiz uso da biblioteca pandas para carregar e manipular os dados dos arquivos CSV.
Utilizei scikit-learn para criar o pipeline de transformação de dados e treinar o(s) modelo(s) necessário(s).
Incluí visualizações e análises preliminares para melhor compreensão dos dados.
Os códigos estão divididos em estapas para sequênciais numeradas e está devidamente comentado para explicar cada etapa da solução abordada.

Sinta-se à vontade para entrar em contato caso tenha alguma dúvida ou sugestão de melhoria.


<h3>Desenvolvedo por:  </h3>
<div>

![Linkedin Badge](https://img.shields.io/badge/-Eduardo_Bitencourt-blue?style=flat-square&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/bitencourt-eduardo/)
![GitHub Org's stars](https://img.shields.io/github/stars/bitencourt-eduardo?style=social)
</div> 

