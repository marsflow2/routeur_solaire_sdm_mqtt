# routeur_solaire_sdm_mqtt
ceci est en cours de conception,
il manque la partie gradateurs 2 un pour le chauffe eau et un suivant pour un chauffage
 forçage et quelques fonction par le biais de valeurs Mqtt > nodred > Home assistant/domoticz
toute aide est la bienvenue :D
je pense rajouter la récupération de l'heure par NTP pour démarrer le chauffe eau quand il n'y a pas sufisament de soleil
je ne mets pas de led ni d'écran, les infos seront dirrectement sur home assistant
j'utilise freetos ce qui permet d'utiliser l'esp32 sur 2 processeurs différents, l'un sur la gestion du routeur et la récupération des valeurs du compteurs sdm
et le second sur la connection réseau/mqtt et la récetion/envoie des valeurs

ce qui est déja mis en place 
l'envoie au broker mqtt des informations suivante

SDM_PHASE_1_VOLTAGE
SDM_PHASE_1_CURRENT
SDM_PHASE_1_APPARENT_POWER
SDM_PHASE_1_REACTIVE_POWER
SDM_FREQUENCY
SDM_PHASE_1_POWER
SDM_EXPORT_ACTIVE_ENERGY
SDM_IMPORT_ACTIVE_ENERGY
SDM_PHASE_1_POWER_FACTOR
thermocouple pour le chauffe eau

la reconnection du wifi auto et mqtt
