
# Guia de instalação

Para instalar o modelo basta Executar o instalador de preferência como Administrador.

 É importante que a pasta edgv_3_orto esteja no mesmo caminho que o instalador.
--------------------------------------------------------------------------------------------
Após a execução não deve aparecer nada, no entanto ao fechar e abrir o QGIS consulte na caixa de processamento se os modelos estão presentes.


O instalador basicamente copia a pasta edgv_3_orto e aponta ela para pasta models do QGIS
 então se o procedimento não for bem sucedido, terá de realizar o processo manualmente.


-------------------------------------------------------------------------------------------
Os arquivos de workflow presentes devem ser utilizado de acordo com a escala desejada,
Basta abrir o DSGTools> Ferramentas de produção > Ferramenta de validação de dados geoespaciais.

Importe o arquivo.



## Deploy

Para fazer o deploy desse projeto rode



## Codigo fonte

import shutil
import os
* Caminho da pasta a ser copiada
_src_folder = './edgv_3_orto'_
* Caminho da pasta de destino
_dst_folder = os.path.join(os.getenv('APPDATA'), 'QGIS', 'QGIS3', 'profiles', 'default', 'processing' ,'model nos')_
* Copia a pasta

_shutil.copytree(src_folder, os.path.join(dst_folder, os.path.basename(src_folder)))
print('Instalado com sucesso!')_
