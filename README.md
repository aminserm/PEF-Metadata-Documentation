# Portail Epidemiologie France (PEF) - XML Export Documentation


## Root

| tag                                          | description                     | link                                     |
| -------------------------------------------- | ------------------------------- | ---------------------------------------- |
| ```<?xml version="1.0" encoding="UTF-8"?>``` | Encoding of the XML file        |                                          |
| ```<FichePortailEpidemiologieFrance> ```     | Entry point of the PEF document | [link](#FichePortailEpidemiologieFrance) |

## FichePortailEpidemiologieFrance

| tag                         | description                                           | link                 |
| --------------------------- | ----------------------------------------------------- | -------------------- |
| ```<Metadonnees>```         | Internal metadata of the resource in the  PEF catalog | [link](#metadonnees) |
| ```<General>```             | ....                                                  | ....                 |
| ```<Caracteristiques>```    | ....                                                  | ....                 |
| ```<Collecte>```            | ....                                                  | ....                 |
| ```<ValorisationEtAcces>``` | ....                                                  | ....                 |

### Metadonnées 

| tag                                 | description                                | type        | link |
| ----------------------------------- | ------------------------------------------ | ----------- | ---- |
| ```<ID>```                          | ID of the reference within the PEF catalog | id          |      |
| ```<VersionFR>```                   | ....                                       | code        |      |
| ```<VersionEN>```                   | ....                                       | code        |      |
| ```<DateCreationFicheFR>```         | ....                                       | date        |      |
| ```<DateCreationFicheEN>```         | ....                                       | date        |      |
| ```<StatutFicheFR>```               | ....                                       | categorical |      |
| ```<StatutFicheEN>```               | ....                                       | categorical |      |
| ```<DateChangementStatutFicheFR>``` | ....                                       | date        |      |
| ```<DateChangementStatutFicheEN>``` | ....                                       | date        |      |
| ```<Auteur>```                      | ....                                       | text        |      |
| ```<UrlFicheFR>```                  | ....                                       | url         |      |
| ```<UrlFicheEN>```                  | ....                                       | url         |      |
| ```<UrlXml>```                      | ....                                       | url         |      |


### General

| tag                                  | description | type        | link                                 |
| ------------------------------------ | ----------- | ----------- | ------------------------------------ |
| ```<Identification>```               | ...         | id          | [link](#generalidentification)       |
| ```<ThematiquesGenerales>```         | ....        | code        | [link](#generalthematiquesgenerales) |
| ```<ResponsableScientifique>```      | ....        | code        |                                      |
| ```<Collaborations>```               | ....        | date        |                                      |
| ```<Financements>```                 | ....        | date        |                                      |
| ```<GouvernanceDeLaBaseDeDonnees>``` | ....        | categorical |                                      |
| ```<ContactSupplementaire>```        | ....        | categorical |                                      |


### General - Identification
| tag                   | description | type | link |
| --------------------- | ----------- | ---- | ---- |
| ``` <NomFR>```        | ...         | text |      |
| ``` <NomEN>```        | ...         | text |      |
| ``` <AcronymeFR>```   | ...         | text |      |
| ``` <AcronymeEN>```   | ...         | text |      |
| ``` <NumeroCnilFR>``` | ...         | text |      |
| ``` <NumeroCnilEN>``` | ...         | text |      |


### General - ThematiquesGenerales

| tag                                   | description | type                  | link |
| ------------------------------------- | ----------- | --------------------- | ---- |
| ``` <DomainesDePathologiesFR>```      | ...         | ```<value>``` list    |      |
| ``` <DomainesDePathologiesEN>```      | ...         | ```<value>``` list    |      |
| ``` <CovidFR>```                      | ...         | categorical (Oui/Non) |      |
| ``` <CovidEN>```                      | ...         | categorical (Yes/No)  |      |
| ``` <PathologiesFR>```                | ...         | text                  |      |
| ``` <PathologiesEN>```                | ...         | text                  |      |
| ``` <DeterminantsDeSanteFR>```        | ...         | ```<value>``` list    |      |
| ``` <DeterminantsDeSanteEN>```        | ...         | ```<value>``` list    |      |
| ``` <DomainesMedicauxPrecisionsFR>``` | ...         | text                  |      |
| ``` <DomainesMedicauxPrecisionsEN>``` | ...         | text                  |      |
| ``` <MotsClesFR>```                   | ...         | ```<value>``` list    |      |
| ``` <MotsClesEN>```                   | ...         | ```<value>``` list    |      |


### General - ResponsableScientifique

| tag                                | description | type               | link |
| ---------------------------------- | ----------- | ------------------ | ---- |
| ``` <ResponsableScientifiqueFR>``` | ...         | ```<value>``` list |      |
| ``` <ResponsableScientifiqueEN>``` | ...         | ```<value>``` list |      |


#### General - ResponsableScientifique - ResponsableScientifiqueFR

| tag                             | description | type | link |
| ------------------------------- | ----------- | ---- | ---- |
| ``` <NomResponsable>```         | ...         | text |      |
| ``` <PrenomResponsable>```      | ...         | text |      |
| ``` <AdresseResponsable>```     | ...         | text |      |
| ``` <TelephoneResponsable>```   | ...         | text |      |
| ``` <MailResponsable>```        | ...         | text |      |
| ``` <LaboratoireResponsable>``` | ...         | text |      |
| ``` <OrganismeResponsable>```   | ...         | text |      |

#### General - ResponsableScientifique - ResponsableScientifiqueEN

| tag                             | description | type | link |
| ------------------------------- | ----------- | ---- | ---- |
| ``` <NomResponsable>```         | ...         | text |      |
| ``` <PrenomResponsable>```      | ...         | text |      |
| ``` <AdresseResponsable>```     | ...         | text |      |
| ``` <TelephoneResponsable>```   | ...         | text |      |
| ``` <MailResponsable>```        | ...         | text |      |
| ``` <LaboratoireResponsable>``` | ...         | text |      |
| ``` <OrganismeResponsable>```   | ...         | text |      |


### General - Collaborations

| tag                                        | description | type | link |
| ------------------------------------------ | ----------- | ---- | ---- |
| ``` <PartenariatsEtReseauxFR>```           | ...         | ?    |      |
| ``` <PartenariatsEtReseauxFR>```           | ...         | ?    |      |
| ``` <PartenariatsEtReseauxPrecisionsFR>``` | ...         | ?    |      |
| ``` <PartenariatsEtReseauxPrecisionsEN>``` | ...         | ?    |      |
| ``` <AutresCollaborationsFR>```            | ...         | ?    |      |
| ``` <AutresCollaborationsEN>```            | ...         | ?    |      |


