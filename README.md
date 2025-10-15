# Arbeidskrav 1: Beskrive data og reproduserbare rapporter

## Prosjektbeskrivelse 
Vi har utført en case-studie av en elitesprintersyklist og effekten av 
tre uker med styrketrening på maksimalt dreiemoment målt med 
isokinetisk dynamometer

## Forfattere
- Ketil Barstad
- Laurits Holden
- Herman Evensen
- Theodor Skinnarland

## Nødvendige programmer 
- R-studio (v. 4.3.1 eller nyere)
- Quarto
- Excel

## Mappestruktur
    Arbeidskrav 1/
    |---Data/ #Rådata i form av Excel-filer
    |---Figurer/ #Figurer fra analysen
    |---Humac_analyse.html #HTML-filen som genereres når man trykker
                           #på render etter å ha åpnet Quarto-dok
    |---Humac_analyse.qmd #Quarto dokumentet med R-kode
    |---README.md

## Hvordan utføre analysen

- Installer følgende pakker i rstudio: 
  install.packages(c("tidyverse", "readxl"))

- Klon repositorien
  git clone https://github.com/KetilBarstad/Arbeidskrav1.git
  
- Last inn pakkene i Rstudio. 
  library(tidyverse)
  library(readxl)
  
- Åpne Humac_analyse.qmd filen i Rstudio, og trykk på "render"
  for å generere en HTML-rapport
  
- Alternativ hvis man ønsker å kjøre koden selv:
  
  Kjør r-scriptet i chunk 1 i Humac_analyse.qmd for å 
  generere datasettet fra rådataene
  
  Kjør de resterende chunks i rekkefølge 
  
  
