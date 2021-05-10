# redis-examples-azure-and-docker

Tres Ejemplos para uso de Redis Cache en Azure y en Javascript

## Prerequisitos: 

Crear Azure Cache for Redis, usando Azure Portal UI or commandline Interface en UI o local

````sh
az group create -n cache-demo-rg -l eastus
# --name = será dns del servicio debe ser único
az redis create --l eastus --name cache-demo --resource-group cache-demo-rg --sku Basic --vm-size c0
````

## src/ContosoTeamStats-AspNetCore

## src/Redistest-CommandLineNetCore

## src/Javascript
Este ejemplo utiliza docker local para ejecutar redis, explicitamente no usa contraseña, solo apropiado para ambientes de desarrollo y testing

Prerequisitos: 

````sh
docker-compose up -d
docker-compose down 

````
