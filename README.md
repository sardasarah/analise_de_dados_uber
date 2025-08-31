# Análise de dados Uber
**Objetivo:** Confirmar hipóteses para o levantamento de insights através da visualização de dados da empresa Uber.

## Fonte dos dados

Para esta análise foi utilizado um arquivo CSV "dados_uber.csv" da plataforma de dados Kaggle.

## Ferramentas

- Linguagem Python no Google Colab

## Fase 1 

Nessa fase, exploramos as tabelas do nosso dataset para formular hipóteses do tema.

**Código em Python**

```python
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
import datetime as dt

df = pd.read_csv('/content/dados_uber.csv')

df.head()

#Saída
Date	Time	Booking ID	Booking Status	Customer ID	Vehicle Type	Pickup Location	Drop Location	Avg VTAT	Avg CTAT	...	Reason for cancelling by Customer	Cancelled Rides by Driver	Driver Cancellation Reason	Incomplete Rides	Incomplete Rides Reason	Booking Value	Ride Distance	Driver Ratings	Customer Rating	Payment Method
0	2024-03-23	12:29:38	"CNR5884300"	No Driver Found	"CID1982111"	eBike	Palam Vihar	Jhilmil	NaN	NaN	...	NaN	NaN	NaN	NaN	NaN	NaN	NaN	NaN	NaN	NaN
1	2024-11-29	18:01:39	"CNR1326809"	Incomplete	"CID4604802"	Go Sedan	Shastri Nagar	Gurgaon Sector 56	4.9	14.0	...	NaN	NaN	NaN	1.0	Vehicle Breakdown	237.0	5.73	NaN	NaN	UPI
2	2024-08-23	08:56:10	"CNR8494506"	Completed	"CID9202816"	Auto	Khandsa	Malviya Nagar	13.4	25.8	...	NaN	NaN	NaN	NaN	NaN	627.0	13.58	4.9	4.9	Debit Card
3	2024-10-21	17:17:25	"CNR8906825"	Completed	"CID2610914"	Premier Sedan	Central Secretariat	Inderlok	13.1	28.5	...	NaN	NaN	NaN	NaN	NaN	416.0	34.02	4.6	5.0	UPI
4	2024-09-16	22:08:00	"CNR1950162"	Completed	"CID9933542"	Bike	Ghitorni Village	Khan Market	5.3	19.6	...	NaN	NaN	NaN	NaN	NaN	737.0	48.21	4.1	4.3	UPI
5 rows × 21 columns

df.shape

df.info()
```
