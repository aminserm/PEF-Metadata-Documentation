# Portail Epidemiologie France (PEF) - XML Export Documentation



## FichePortailEpidemiologieFrance

| tag                         | description                                           | detail                       |
| --------------------------- | ----------------------------------------------------- | ---------------------------- |
| ```<Metadonnees>```         | Internal metadata of the resource in the  PEF catalog | [link](#metadonnees)         |
| ```<General>```             | ....                                                  | [link](#general)             |
| ```<Caracteristiques>```    | ....                                                  | [link](#caracteristiques)    |
| ```<Collecte>```            | ....                                                  | [link](#collecte)            |
| ```<ValorisationEtAcces>``` | ....                                                  | [link](#valorisationetacces) |


### Metadonnées  

| tag                                 | description                                | type        | detail |
| ----------------------------------- | ------------------------------------------ | ----------- | ------ |
| ```<ID>```                          | ID of the reference within the PEF catalog | id          |        |
| ```<VersionFR>```                   | ....                                       | code        |        |
| ```<VersionEN>```                   | ....                                       | code        |        |
| ```<DateCreationFicheFR>```         | ....                                       | date        |        |
| ```<DateCreationFicheEN>```         | ....                                       | date        |        |
| ```<StatutFicheFR>```               | ....                                       | categorical |        |
| ```<StatutFicheEN>```               | ....                                       | categorical |        |
| ```<DateChangementStatutFicheFR>``` | ....                                       | date        |        |
| ```<DateChangementStatutFicheEN>``` | ....                                       | date        |        |
| ```<Auteur>```                      | ....                                       | text        |        |
| ```<UrlFicheFR>```                  | ....                                       | url         |        |
| ```<UrlFicheEN>```                  | ....                                       | url         |        |
| ```<UrlXml>```                      | ....                                       | url         |        |



### General

| tag                                  | description | type        | detail                                          |
| ------------------------------------ | ----------- | ----------- | ----------------------------------------------- |
| ```<Identification>```               | ...         | id          | [link](#general---identification)               |
| ```<ThematiquesGenerales>```         | ....        | code        | [link](#general---thematiquesgenerales)         |
| ```<ResponsableScientifique>```      | ....        | code        | [link](#general---responsablescientifique)      |
| ```<Collaborations>```               | ....        | date        | [link](#general---collaborations)               |
| ```<Financements>```                 | ....        | date        | [link](#general---financements)                 |
| ```<GouvernanceDeLaBaseDeDonnees>``` | ....        | categorical | [link](#general---gouvernancedelabasededonnees) |
| ```<ContactSupplementaire>```        | ....        | categorical | [link](#general---contactsupplementaire)        |


#### General - Identification
| tag                   | description | type | detail |
| --------------------- | ----------- | ---- | ------ |
| ``` <NomFR>```        | ...         | text |        |
| ``` <NomEN>```        | ...         | text |        |
| ``` <AcronymeFR>```   | ...         | text |        |
| ``` <AcronymeEN>```   | ...         | text |        |
| ``` <NumeroCnilFR>``` | ...         | text |        |
| ``` <NumeroCnilEN>``` | ...         | text |        |


#### General - ThematiquesGenerales

| tag                                   | description | type                  | detail |
| ------------------------------------- | ----------- | --------------------- | ------ |
| ``` <DomainesDePathologiesFR>```      | ...         | ```<value>``` list    |        |
| ``` <DomainesDePathologiesEN>```      | ...         | ```<value>``` list    |        |
| ``` <CovidFR>```                      | ...         | categorical (Oui/Non) |        |
| ``` <CovidEN>```                      | ...         | categorical (Yes/No)  |        |
| ``` <PathologiesFR>```                | ...         | text                  |        |
| ``` <PathologiesEN>```                | ...         | text                  |        |
| ``` <DeterminantsDeSanteFR>```        | ...         | ```<value>``` list    |        |
| ``` <DeterminantsDeSanteEN>```        | ...         | ```<value>``` list    |        |
| ``` <DomainesMedicauxPrecisionsFR>``` | ...         | text                  |        |
| ``` <DomainesMedicauxPrecisionsEN>``` | ...         | text                  |        |
| ``` <MotsClesFR>```                   | ...         | ```<value>``` list    |        |
| ``` <MotsClesEN>```                   | ...         | ```<value>``` list    |        |


#### General - ResponsableScientifique

| tag                                | description | type               | detail |
| ---------------------------------- | ----------- | ------------------ | ------ |
| ``` <ResponsableScientifiqueFR>``` | ...         | ```<value>``` list |        |
| ``` <ResponsableScientifiqueEN>``` | ...         | ```<value>``` list |        |


##### General - ResponsableScientifique - ResponsableScientifiqueFR

| tag                             | description | type | detail |
| ------------------------------- | ----------- | ---- | ------ |
| ``` <NomResponsable>```         | ...         | text |        |
| ``` <PrenomResponsable>```      | ...         | text |        |
| ``` <AdresseResponsable>```     | ...         | text |        |
| ``` <TelephoneResponsable>```   | ...         | text |        |
| ``` <MailResponsable>```        | ...         | text |        |
| ``` <LaboratoireResponsable>``` | ...         | text |        |
| ``` <OrganismeResponsable>```   | ...         | text |        |

##### General - ResponsableScientifique - ResponsableScientifiqueEN

| tag                             | description | type | detail |
| ------------------------------- | ----------- | ---- | ------ |
| ``` <NomResponsable>```         | ...         | text |        |
| ``` <PrenomResponsable>```      | ...         | text |        |
| ``` <AdresseResponsable>```     | ...         | text |        |
| ``` <TelephoneResponsable>```   | ...         | text |        |
| ``` <MailResponsable>```        | ...         | text |        |
| ``` <LaboratoireResponsable>``` | ...         | text |        |
| ``` <OrganismeResponsable>```   | ...         | text |        |


#### General - Collaborations

| tag                                        | description | type | detail |
| ------------------------------------------ | ----------- | ---- | ------ |
| ``` <PartenariatsEtReseauxFR>```           | ...         | ?    |        |
| ``` <PartenariatsEtReseauxFR>```           | ...         | ?    |        |
| ``` <PartenariatsEtReseauxPrecisionsFR>``` | ...         | ?    |        |
| ``` <PartenariatsEtReseauxPrecisionsEN>``` | ...         | ?    |        |
| ``` <AutresCollaborationsFR>```            | ...         | ?    |        |
| ``` <AutresCollaborationsEN>```            | ...         | ?    |        |


#### General - Financements

| tag                               | description | type | detail |
| --------------------------------- | ----------- | ---- | ------ |
| ``` <TypeDeFinancementsFR>```     | ...         | ?    |        |
| ``` <TypeDeFinancementsEN>```     | ...         | ?    |        |
| ``` <FinancementsPrecisionsFR>``` | ...         | ?    |        |
| ``` <FinancementsPrecisionsEN>``` | ...         | ?    |        |

#### General - GouvernanceDeLaBaseDeDonnees

| tag                                   | description | type                  | detail |
| ------------------------------------- | ----------- | --------------------- | ------ |
| ``` <OrganisationFR>```               | ...         | ```<value>``` list    |        |
| ``` <OrganisationEN>```               | ...         | ```<value>``` list    |        |
| ``` <ExistenceDeComiteFR>```          | ...         | categorical (Oui/Non) |        |
| ``` <ExistenceDeComiteEN>```          | ...         | categorical (Yes/No)  |        |
| ``` <LabellisationsEtExpertisesFR>``` | ...         | ?                     |        |
| ``` <LabellisationsEtExpertisesEN>``` | ...         | ?                     |        |

##### General - GouvernanceDeLaBaseDeDonnees - OrganisationFR

| tag                         | description | type | detail |
| --------------------------- | ----------- | ---- | ------ |
| ``` <Organisation>```       | ...         | text |        |
| ``` <StatutOrganisation>``` | ...         | text |        |

##### General - GouvernanceDeLaBaseDeDonnees - OrganisationEN

| tag                         | description | type | detail |
| --------------------------- | ----------- | ---- | ------ |
| ``` <Organisation>```       | ...         | text |        |
| ``` <StatutOrganisation>``` | ...         | text |        |


#### General - ContactSupplementaire

| tag                              | description | type               | detail |
| -------------------------------- | ----------- | ------------------ | ------ |
| ``` <ContactSupplementaireFR>``` | ...         | ```<value>``` list |        |
| ``` <ContactSupplementaireEN>``` | ...         | ```<value>``` list |        |


##### General - ContactSupplementaire - ContactSupplementaireFR

| tag                            | description | type | detail |
| ------------------------------ | ----------- | ---- | ------ |
| ``` <ContactSupplementaire>``` | ...         | ?    |        |
| ``` <PrenomContact>```         | ...         | ?    |        |
| ``` <AdresseContact>```        | ...         | ?    |        |
| ``` <TelephoneContact>```      | ...         | ?    |        |
| ``` <MailContact>```           | ...         | ?    |        |
| ``` <LaboratoireContact>```    | ...         | ?    |        |
| ``` <OrganismeContact>```      | ...         | ?    |        |

##### General - ContactSupplementaire - ContactSupplementaireEN

| tag                            | description | type | detail |
| ------------------------------ | ----------- | ---- | ------ |
| ``` <ContactSupplementaire>``` | ...         | ?    |        |
| ``` <PrenomContact>```         | ...         | ?    |        |
| ``` <AdresseContact>```        | ...         | ?    |        |
| ``` <TelephoneContact>```      | ...         | ?    |        |
| ``` <MailContact>```           | ...         | ?    |        |
| ``` <LaboratoireContact>```    | ...         | ?    |        |
| ``` <OrganismeContact>```      | ...         | ?    |        |


### Caracteristiques

| tag                                | description | type | detail |
| ---------------------------------- | ----------- | ---- | ------ |
| ``` <TypeDeBaseDeDonnees>```       | ...         | tag  |        |
| ``` <ObjectifDeLaBaseDeDonnees>``` | ...         | ?    |        |
| ``` <TypeDePopulation>```          | ...         | ?    |        |


#### Caracteristiques - TypeDeBaseDeDonnees

| tag                                        | description | type               | detail |
| ------------------------------------------ | ----------- | ------------------ | ------ |
| ``` <TypeDeBaseFR>```                      | ...         | ```<value>``` list |        |
| ``` <TypeDeBaseEN>```                      | ...         | ```<value>``` list |        |
| ``` <TypeDeBaseAutreFR>```                 | ...         | ?                  |        |
| ``` <TypeDeBaseAutreEN>```                 | ...         | ?                  |        |
| ``` <TypeEnqueteFR>```                     | ...         | ```<value>``` list |        |
| ``` <TypeEnqueteEN>```                     | ...         | ```<value>``` list |        |
| ``` <RecrutementParIntermediaireFR>```     | ...         | ```<value>``` list |        |
| ``` <RecrutementParIntermediaireEN>```     | ...         | ```<value>``` list |        |
| ``` <BaseOuRegistrePrecisionsFR>```        | ...         | ?                  |        |
| ``` <BaseOuRegistrePrecisionsEN>```        | ...         | ?                  |        |
| ``` <RecrutementSurBaseFR>```              | ...         | ```<value>``` list |        |
| ``` <RecrutementSurBaseEN>```              | ...         | ```<value>``` list |        |
| ``` <EnqueteInterventionnelleFR>```        | ...         | ?                  |        |
| ``` <EnqueteInterventionnelleEN>```        | ...         | ?                  |        |
| ``` <InterventionnellePrecisionsFR>```     | ...         | ```<value>``` list |        |
| ``` <InterventionnellePrecisionsEN>```     | ...         | ```<value>``` list |        |
| ``` <ModaliteConstitutionEchantillonFR>``` | ...         | text               |        |
| ``` <ModaliteConstitutionEchantillonEN>``` | ...         | text               |        |


#### Caracteristiques - ObjectifDeLaBaseDeDonnees

| tag                          | description | type | detail |
| ---------------------------- | ----------- | ---- | ------ |
| ``` <ObjectifGeneralFR>```   | ...         | text |        |
| ``` <ObjectifGeneralEN>```   | ...         | text |        |
| ``` <CriteresInclusionFR>``` | ...         | text |        |
| ``` <CriteresInclusionEN>``` | ...         | text |        |

#### Caracteristiques - TypeDePopulation

| tag                                    | description | type               | detail |
| -------------------------------------- | ----------- | ------------------ | ------ |
| ``` <TranchesAgeFR>```                 | ...         | ```<value>``` list |        |
| ``` <TranchesAgeEN>```                 | ...         | ```<value>``` list |        |
| ``` <PopulationFR>```                  | ...         | ```<value>``` list |        |
| ``` <PopulationEN>```                  | ...         | ```<value>``` list |        |
| ``` <PopulationCimFR>```               | ...         | ```<value>``` list |        |
| ``` <PopulationCimEN>```               | ...         | ```<value>``` list |        |
| ``` <SexeFR>```                        | ...         | ```<value>``` list |        |
| ``` <SexeEN>```                        | ...         | ```<value>``` list |        |
| ``` <ChampGeographiqueFR>```           | ...         | ```<value>``` list |        |
| ``` <ChampGeographiqueEN>```           | ...         | ```<value>``` list |        |
| ``` <RegionsConcerneesFR>```           | ...         | ```<value>``` list |        |
| ``` <RegionsConcerneesEN>```           | ...         | ```<value>``` list |        |
| ``` <ChampGeographiquePrecisionsFR>``` | ...         | text               |        |
| ``` <ChampGeographiquePrecisionsEN>``` | ...         | text               |        |

##### Caracteristiques - TypeDePopulation - PopulationCimFR

| tag          | description | type | detail |
| ------------ | ----------- | ---- | ------ |
| ``` <Cim>``` | ...         | text |        |

##### Caracteristiques - TypeDePopulation - PopulationCimEN

| tag          | description | type | detail |
| ------------ | ----------- | ---- | ------ |
| ``` <Cim>``` | ...         | text |        |



