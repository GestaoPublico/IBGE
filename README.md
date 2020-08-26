# IBGE
 
### Como utilizar API IBGE

A seguinte codificação adotada pelo IBGE deverá ser utilizada para representar o código da UF:

#### Região Norte
* 11-Rondônia/RO
* 12-Acre/AC
* 13-Amazonas/AM
* 14-Roraima/RR
* 15-Pará/PA
* 16-Amapá/AP
* 17-Tocantins/TO

#### Região Nordeste
* 21-Maranhão/MA
* 22-Piauí/PI
* 23-Ceará/CE
* 24-Rio Grande do Norte/RN
* 25-Paraíba/PB
* 26-Pernambuco/PE
* 27-Alagoas/AL
* 28-Sergipe/SE
* 29-Bahia/BA

#### Região Sudeste
* 31-Minas Gerais/MG
* 32-Espírito Santo/ES
* 33-Rio de Janeiro/RJ
* 35-São Paulo/SP

#### Região Sul
* 41-Paraná/PR
* 42-Santa Catarina/SC
* 43-Rio Grande do Sul/RS

#### Região Centro-Oeste
* 50-Mato Grosso do Sul/MS
* 51-Mato Grosso/MT
* 52-Goiás/GO
* 53-Distrito Federal/DF

```https://raw.githubusercontent.com/GestaoPublico/IBGE/master/"""código da UF"""/"""código da municipios""".json```

Apresentar ```{ "cidade": "Alta Floresta D'Oeste", "IBGE":  "1100015", "ESTADO": Rondônia, "ID": 11 }```

```$location = file_get_contents("https://gist.githubusercontent.com/letanure/3012978/raw/2e43be5f86eef95b915c1c804ccc86dc9790a50a/estados-cidades2.json");

$json= json_decode(file_get_contents("https://raw.githubusercontent.com/GestaoPublico/IBGE/master/11/1100015.json"));
echo $json->cidade.'<br>';
echo $json->IBGE.'<br>';
echo $json->ESTADO.'<br>';
echo $json->ID;```


