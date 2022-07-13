# ARI300-RF-GATEWAY by LU4AEY

![alt text](https://raw.githubusercontent.com/hp3icc/ARI300-RF-GATEWAY/main/ari300rf-gateway.jpg)

#

# Descripcion:

ARI300 , es un cliente USRP PC RF Gateway, con tx ptt y rx serial com control, de desarrollo 100% del colega LU4AEY Claudio Zanella, permite utilizar un radio Analogico como nodo conectado a una red Digital, permitiendo a las estaciones que no cuentan con radios digitales , tener comunicacion con redes digitales de radio , desde un sencillo radio analogico.

#

# Instalacion 

descargue el archivo comprimido desde el siguiente link:

<p><a href="https://github.com/hp3icc/ARI300-RF-GATEWAY/blob/main/ARI300_RF_Gateway.zip?raw=true" target="_blank">ARI300-RF-GATEWAY</a></p>

descomprima el archivo descargado y edite los archivos de configuracion remplazando los datos por los suyos 

#

# Configuracion 

Edite los archivos ARI300.ini y DMR_TalkGroups.def , con sus datos, los datos de su server USRP y tg a utilizar:

* ARI300.ini

![alt text](https://raw.githubusercontent.com/hp3icc/ARI300-RF-GATEWAY/main/ARI300INI.jpg)

#

* DMR_TalkGroups.def

![alt text](https://raw.githubusercontent.com/hp3icc/ARI300-RF-GATEWAY/main/DMR_TalkGroups.jpg)

#

# Interface

ARI300, es compatible con cualquier cable o interface conocido utilizado para aplicaciones como Echolink, Zello PC Gateway u otros.

Cada usuario podra editar los pines de comunicacion que utiliza su cable DB9 para TX (PTT) o RX (COS - COR) desde el archivo de configuracion.

Si no cuenta con con un interface o cable , el colega LU4AEY nos comparte un circuito basico y economico , que puede ensamblar por menos de 5 dolares: 

![alt text](https://raw.githubusercontent.com/hp3icc/ARI300-RF-GATEWAY/main/Interface-ARI300--Circuito-Electrico-.jpg)

#

# Nota:

Importante, para que el software identifique la actividad de señal analoga, el radio que utilice como nodo , debe tener pin de cor/cos , y el cable o interface a utilizar debe tener este pin del radio, conectado al Db9 puerto com, pin DCD, o al que a configuado en la linea de cosSignal en el archivo de configuracion.

#

<p>Mas informacion en el siguiente link : <a href="http://www.argentina-room.dns-cloud.net/" target="_blank">Argentina Room</a></p>
