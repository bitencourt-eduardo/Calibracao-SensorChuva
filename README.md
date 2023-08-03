# Calibracao-SensorChuva

# Desafio FieldPRO

<h1 align="center"> <img src="https://user-images.githubusercontent.com/109546269/203450752-f4d42e69-128c-42a3-87e0-6c22bac0fa45.jpg" width=180px></h1>   



<h2>Status do Projeto</h2>

![Badge em Desenvolvimento](http://img.shields.io/static/v1?label=STATUS&message=EM%20DESENVOLVIMENTO&color=GREEN&style=for-the-badge)
![GitHub Org's stars](https://img.shields.io/github/stars/camilafernanda?style=social)

# Índice
<!--ts-->
   * [Sobre](#sobre)
   * [Requisitos](#requisitos)
   * [Estruturação de Dados](#estruturação-de-dados)
   * [Documentação da API](#documentação-da-api)
       * [Cadastro do cliente](#cadastro-do-cliente)
       * [Rota de Contas](#rota-de-contas)
       * [Rotas de Endereço](#rotas-de-endereço)
       * [Rotas de Transações](#rotas-de-transações)
   * [Ferramentas e Tecnologias](#ferramentas-e-tecnologias)
 
<!--te-->
 
 # 🧾Sobre
 
 Desenvolvimento de API de simulação de banco, com operações bancárias do dia a dia, obedencendo algumas entregas mínimas como:
  
  
- [x] Cadastro de Clientes<br>
- [x] Buscar os Clientes Cadastrados<br>
- [x] Transferências de saldo entre as contas<br>
- [x] Buscar o histórico de transações entre as contas<br>

# Requisitos 

<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/java/java-original.svg" width="50" height="50"/> <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/mysql/mysql-original.svg" width="40" height="40"/> <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/intellij/intellij-original.svg" width="40" height="40"/><img src="https://cdn.worldvectorlogo.com/logos/postman.svg" width="40" height="40"/>

* Ter instalado na sua máquina: MySQL, uma IDE (recomendamos o Intellij) e Java.
* Como rodar a aplicação: Clone este repositório
* Configure o arquivo application.properties com seu dados pessoais do Banco de dados de MySql: o SQL para popular o banco de dados no MySQL Workbench se encontra na pasta `bancoDeDados` e o arquivo é chamado de `bd_divasbank.sql`.
* Caso prefira utilizar o banco de dados H2, o projeto já possui esta dependência.
* Acesse a pasta do projeto no terminal/cmd e vá para a pasta do Divas Bank,
* Execute a aplicação: o servidor entra pela porta 8080.


# Estruturação de Dados


| Parâmetro   | Tipo       | Descrição                           |
| :---------- | :--------- | :---------------------------------- |
| `valor` | `String` | **Obrigatório** |
| `numeroContaOrigem` | `String` | **Obrigatório**. |
| `numeroContaDestino`| `String` | **Obrigatório**. |
| `tipoTransacao` | `String` | O tipoTransacao é enviado automaticamente e seu valor Default é "transaferencia". Pois no momento é a única transação que o projeto realiza.|
| `data` | `Date` | A data da transação é enviada automaticamente.|


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

<h3>Desenvolvedo por:  </h3>
<div>

![Linkedin Badge](https://img.shields.io/badge/-Eduardo_Bitencourt-blue?style=flat-square&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/bitencourt-eduardo/)
</div>
