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
