# ARI300-RF-GATEWAY by LU4AEY

![alt text](https://raw.githubusercontent.com/hp3icc/ARI300-RF-GATEWAY/main/ari300rf-gateway.jpg)

#

# Descripcion:

ARI300 , es un cliente USRP PC RF Gateway, de desarrollo 100% del colega LU4AEY Claudio Zanella, permite utilizar un radio Analogico como nodo conectado a una red Digital, permitiendo a las estaciones que no cuentan con radios digitales , tener comunicacion con redes digitales de radio , desde un sencillo radio analogico.

#

# Instalacion 

descargue el archivo comprimido desde el siguiente link:

<p><a href="https://github.com/hp3icc/ARI300-RF-GATEWAY/blob/main/ARI300_RF_Gateway.zip?raw=true" target="_blank">ARI300-RF-GATEWAY</a></p>

descomprima el archivo descargado y edite los archivos de configuracion remplazando los datos por los suyos 

#

# Interface

ARI300, es compatible con cualquier cable o interface conocido utilizado para aplicaciones como Echolink, Zello PC Gateway u otros.

Cada usuario podra editar los pines de comunicacion que utiliza su cable DB9 para TX (PTT) o RX (COS - COR) desde el archivo de configuracion.

Si no cuenta con con un interface o cable , el colega LU4AEY nos comparte un circuito basico y economico , que puede ensamblar por menos de 5 dolares: 

![alt text](https://raw.githubusercontent.com/hp3icc/ARI300-RF-GATEWAY/main/Interface-ARI300--Circuito-Electrico-.jpg)

#

# Configuracion 

Edite los archivos ARI300.ini y DMR_TalkGroups.def , con sus datos, los datos de su server USRP y tg a utilizar:

* ARI300.ini

[General]

Callsign=HP3ICC               : Callsign

subscriberID=1234567          : DMRiD

repeaterID=123456789          : DMRid + 2 digitos del 01-99

pttInterface=com1             : Db9 Puerto serial Com

pttSignal=dsr                 : pin db9 activa circuito ptt

cosSignal=dcd                 : pin db9 activa rx (cos/cor)

usrpAddress=192.168.100.10    : ip o url de servidor Usrp

usrpTxPort=50001              : Puerto Usrp TX

usrpRxPort=50001              : Puerto Usrp RX

defaultMode=DMR               

defaultTG=99999               : TG predeterminado de Transmision

userMode=0                    : 0 = Modo bridge radio Gateway, 1 = Modo Direct PC

useFilter=1                   

tot=5                         : Time off Tx radio

slot=2                        

quindar_tones=1               : Tono de cortesia analogo

Jitter=300                    

inp_index=0

out_index=0

rx_level=1

tx_level=1



* DMR_TalkGroups.def

##############################################
#Lista de tg que se muestran en la aplicacion#
##############################################

722;Argentina

7221;Arg AMBA

7229;Arg Room


#

# Nota:

Importante, para que el software identifique la actividad de señal analoga, el radio que utilice como nodo , debe tener pin de cor/cos , y el cable o interface a utilizar debe tener este pin conectado al db9 en cualquiera de las 3 configuraciones : CDC , CTS, DSR.

#

<p>Mas informacion en el siguiente link : <a href="http://www.argentina-room.dns-cloud.net/" target="_blank">Argentina Room</a></p>
