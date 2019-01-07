# Instruções


Primeiramente criei uma base de dados no SQL Server e criei uma tabela conforme modelo de estrutura no arquivo *readme.html* enviado.

Segue código utilizado para criação do mesmo:


```SQL
CREATE DATABASE MAXMI
GO

CREATE TABLE BUSCAS (
	id VARCHAR(21) PRIMARY KEY NOT NULL,
	idusers BIGINT,
	idsearch VARCHAR(21),
	companhia_aerea VARCHAR(7),
	tipo_de_voo VARCHAR(9),
	airportfrom VARCHAR(5),
	airportto VARCHAR(5),
	data_ida DATETIME,
	data_volta DATETIME,
	dias_entre_a_viagem BIGINT,
	adults BIGINT,
	child BIGINT,
	infants BIGINT,
	countrydeparture VARCHAR(2),
	countryarrival VARCHAR(2),
	voo_internation VARCHAR(3),
	direcao VARCHAR(14),
	classe VARCHAR(11),
	created DATETIME,
	data_inicio_buscador DATETIME,
	data_fim_buscador DATETIME,
	data_recebimento_busca DATETIME,
	diffsecstartedended INT,
	diffsecendedreceived INT,
	qtyflights BIGINT,
	qtyreceived BIGINT,
	qtyBetterPriceInAirline INT,
	qtyBetterPriceInMM INT,
	cheapestInMMGo BIT,
	cheapestInMMReturn BIT,
	nome_aeroporto_ida VARCHAR(100),
	codinome_aeroporto_ida VARCHAR(100),
	combinacao_aeroporto_ida VARCHAR(50),
	grupo_aeroporto_ida VARCHAR(3),
	nome_aeroporto_volta VARCHAR(100),
	codinome_aeroporto_volta VARCHAR(100),
	combinacao_aeroporto_volta VARCHAR(50),
	grupo_aeroporto_volta VARCHAR(3)
	)
```

Após a criação da tabela, importei o arquivo *out.csv* enviado para dentro da tabela *BUSCAS*.


Através do *Power BI* criei uma conexão com a base no SQL Server e elaborei alguns Dashboards com algumas análises que podem ser conferidas através do link abaixo.


[Interactive Viz](http://bit.ly/MaxMi-Analise)

Ou no arquivo [ANALISES.md](ANALISES.md)
