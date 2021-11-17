# Spatial Suite toolbox

Det her plugin kan bruges til at lave xml snippets, som er 95% klare til at blive kopieret i diverse xml konfigurationsfiler. Plugin'et kan lave xml snippets til en datasource, theme, presentation og target. Der er nogle ting, som man skal ændre før man kopierer sin snippet ind. Det kan man læse nedenfor.

Datasættet skal være i en [[PostgreSQL]] database før det virker.

Det her er work in progress :) 

## Installation

Download en zip fil fra det her repo ved at klikke på den grønne _Code_ knap og så _Download ZIP_. Brug så muligheden for at installere et plugin fra en ZIP fil i QGIS.

Plugin'et virker kun med python 3.9, som er installeret med QGIS version 3.22.

## Datasource

Laver en enkelt datasource, som er klar til at blive kopieret ind i en _datasources.xml_ fil i et modul.

Lige nu, så er endpoint navnet hardkodet ind i systemet, så det skal man huske at ændre. Se [Issue #2](https://github.com/Slagelse-GIS/sps_qgis_toolbox/issues/2).

## Theme

Laver en meget grundlæggende theme xml. Den eksporterer ikke styling med over, men giver det bare en vilkårlig rgb værdi.

Her skal man huske at ændre sin metadata tekst i cbinfo-metadata tags.

## Presentation

Laver en presentation, hvor alle kolonner er vist med kolonnenavnene. Den skal nok tilpasses, hvis man vil ændre på labels af hver kolonne.

Man skal også huske at ændre i den allerførste kolonne, som har en `format="heading"` attribut.

## Target

Her skal man huske at ændre modulnavnet i presentation attributten.