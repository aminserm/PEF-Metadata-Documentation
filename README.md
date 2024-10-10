# Portail Epidemiologie France (PEF) - XML Export Documentation



## FichePortailEpidemiologieFrance

| tag                         | description                                           | link                 |
| --------------------------- | ----------------------------------------------------- | -------------------- |
| ```<Metadonnees>```         | Internal metadata of the resource in the  PEF catalog | [link](#metadonnees) |
| ```<General>```             | ....                                                  | ....                 |
| ```<Caracteristiques>```    | ....                                                  | ....                 |
| ```<Collecte>```            | ....                                                  | ....                 |
| ```<ValorisationEtAcces>``` | ....                                                  | ....                 |




<details>
<summary> Metadonnées
 </summary>

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

</details>




### General

| tag                                  | description | type        | link                                       |
| ------------------------------------ | ----------- | ----------- | ------------------------------------------ |
| ```<Identification>```               | ...         | id          | [link](#general---identification)          |
| ```<ThematiquesGenerales>```         | ....        | code        | [link](#general---thematiquesgenerales)    |
| ```<ResponsableScientifique>```      | ....        | code        | [link](#general---responsablescientifique) |
| ```<Collaborations>```               | ....        | date        | [link](#general---collaborations)          |
| ```<Financements>```                 | ....        | date        |                                            |
| ```<GouvernanceDeLaBaseDeDonnees>``` | ....        | categorical |                                            |
| ```<ContactSupplementaire>```        | ....        | categorical |                                            |


#### General - Identification
| tag                   | description | type | link |
| --------------------- | ----------- | ---- | ---- |
| ``` <NomFR>```        | ...         | text |      |
| ``` <NomEN>```        | ...         | text |      |
| ``` <AcronymeFR>```   | ...         | text |      |
| ``` <AcronymeEN>```   | ...         | text |      |
| ``` <NumeroCnilFR>``` | ...         | text |      |
| ``` <NumeroCnilEN>``` | ...         | text |      |


#### General - ThematiquesGenerales

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


#### General - ResponsableScientifique

| tag                                | description | type               | link |
| ---------------------------------- | ----------- | ------------------ | ---- |
| ``` <ResponsableScientifiqueFR>``` | ...         | ```<value>``` list |      |
| ``` <ResponsableScientifiqueEN>``` | ...         | ```<value>``` list |      |


##### General - ResponsableScientifique - ResponsableScientifiqueFR

| tag                             | description | type | link |
| ------------------------------- | ----------- | ---- | ---- |
| ``` <NomResponsable>```         | ...         | text |      |
| ``` <PrenomResponsable>```      | ...         | text |      |
| ``` <AdresseResponsable>```     | ...         | text |      |
| ``` <TelephoneResponsable>```   | ...         | text |      |
| ``` <MailResponsable>```        | ...         | text |      |
| ``` <LaboratoireResponsable>``` | ...         | text |      |
| ``` <OrganismeResponsable>```   | ...         | text |      |

##### General - ResponsableScientifique - ResponsableScientifiqueEN

| tag                             | description | type | link |
| ------------------------------- | ----------- | ---- | ---- |
| ``` <NomResponsable>```         | ...         | text |      |
| ``` <PrenomResponsable>```      | ...         | text |      |
| ``` <AdresseResponsable>```     | ...         | text |      |
| ``` <TelephoneResponsable>```   | ...         | text |      |
| ``` <MailResponsable>```        | ...         | text |      |
| ``` <LaboratoireResponsable>``` | ...         | text |      |
| ``` <OrganismeResponsable>```   | ...         | text |      |


#### General - Collaborations

| tag                                        | description | type | link |
| ------------------------------------------ | ----------- | ---- | ---- |
| ``` <PartenariatsEtReseauxFR>```           | ...         | ?    |      |
| ``` <PartenariatsEtReseauxFR>```           | ...         | ?    |      |
| ``` <PartenariatsEtReseauxPrecisionsFR>``` | ...         | ?    |      |
| ``` <PartenariatsEtReseauxPrecisionsEN>``` | ...         | ?    |      |
| ``` <AutresCollaborationsFR>```            | ...         | ?    |      |
| ``` <AutresCollaborationsEN>```            | ...         | ?    |      |


#### General - Financements

| tag                               | description | type | link |
| --------------------------------- | ----------- | ---- | ---- |
| ``` <TypeDeFinancementsFR>```     | ...         | ?    |      |
| ``` <TypeDeFinancementsEN>```     | ...         | ?    |      |
| ``` <FinancementsPrecisionsFR>``` | ...         | ?    |      |
| ``` <FinancementsPrecisionsEN>``` | ...         | ?    |      |

#### General - GouvernanceDeLaBaseDeDonnees

| tag                                   | description | type                  | link |
| ------------------------------------- | ----------- | --------------------- | ---- |
| ``` <OrganisationFR>```               | ...         | ```<value>``` list    |      |
| ``` <OrganisationEN>```               | ...         | ```<value>``` list    |      |
| ``` <ExistenceDeComiteFR>```          | ...         | categorical (Oui/Non) |      |
| ``` <ExistenceDeComiteEN>```          | ...         | categorical (Yes/No)  |      |
| ``` <LabellisationsEtExpertisesFR>``` | ...         | ?                     |      |
| ``` <LabellisationsEtExpertisesEN>``` | ...         | ?                     |      |

##### General - GouvernanceDeLaBaseDeDonnees - OrganisationFR

| tag                         | description | type | link |
| --------------------------- | ----------- | ---- | ---- |
| ``` <Organisation>```       | ...         | text |      |
| ``` <StatutOrganisation>``` | ...         | text |      |

##### General - GouvernanceDeLaBaseDeDonnees - OrganisationEN

| tag                         | description | type | link |
| --------------------------- | ----------- | ---- | ---- |
| ``` <Organisation>```       | ...         | text |      |
| ``` <StatutOrganisation>``` | ...         | text |      |


#### General - ContactSupplementaire

| tag                              | description | type               | link |
| -------------------------------- | ----------- | ------------------ | ---- |
| ``` <ContactSupplementaireFR>``` | ...         | ```<value>``` list |      |
| ``` <ContactSupplementaireEN>``` | ...         | ```<value>``` list |      |


##### General - GouvernanceDeLaBaseDeDonnees - OrganisationEN

| tag                         | description | type | link |
| --------------------------- | ----------- | ---- | ---- |
| ``` <Organisation>```       | ...         | text |      |
| ``` <StatutOrganisation>``` | ...         | text |      |

##### General - GouvernanceDeLaBaseDeDonnees - OrganisationEN

| tag                         | description | type | link |
| --------------------------- | ----------- | ---- | ---- |
| ``` <Organisation>```       | ...         | text |      |
| ``` <StatutOrganisation>``` | ...         | text |      |





