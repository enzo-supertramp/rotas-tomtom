# rotas_tomtom
Floating Car Data

**Gerar vetor das rotas obtidas via Radares Automotivos**
<br> O script acessa os arquivos gerados via radares automotivos; gera um modelo json para cada rota; carrega os arquivos json; requisita e armazena o valor do jobID de cada um dos arquivos json; requisita e faz o download dos resultados de cada jobID.
<br>
<br> O script divide-se em 3 etapas:
<br>**ETAPA 1:** Define functions para serem usadas em cada arquivo
<br>**ETAPA 2:** Gera os dados jobID em forma de lista (job_id)
<br>**ETAPA 3:** Faz o download dos resultados
<br>**ETAPA 4:** Descompacta e exclui os arquivos zip, mantendo os arquivos GIS e planilha
<br>
<br> obs: Este código foi tratado de uma versão de outra autoria

Os dados obtidos pelo API Traffic Stats da empresa TomTom correspondem a Floating Car Data, que são dados armazenados via geolocalização, essa API se subdivide em três tipos de API: Análise de Rotas (Route Analysis); Análise de Áreas (Area Analysis) e Densidade de Tráfego (Traffic Density). No presente estudo a API de Análise de Rotas foi a escolhida para verificação via linguagem computacional, nela são solicitados como dados de entrada as coordenadas dos pares OD e o período (datas e horários) da viagem em estudo, com isso são gerados o arquivo GIS (Sistema de Informação Geográfica) em formato shapefile (que contém informações vetoriais) da rota em estudo e um arquivo em planilha, no formato .xlsx, que contém as respectivas informações para cada um dos arcos que compõe essa rota como tempo de viagem, velocidade média, distância percorrida entre outros. 
