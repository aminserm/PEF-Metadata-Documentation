# Portail Epidemiologie France (PEF) - XML Export Documentation

This document provides a detailed description of the XML metadata export of the [Portail Epidemiologie France (PEF) catalog](https://epidemiologie-france.aviesan.fr/epidemiologie-france/catalogue).

PEF website provides a glossary of the different metadata sections, in french: [epidemiologie-france.aviesan.fr/epidemiologie-france/ressources/glossaire](https://epidemiologie-france.aviesan.fr/epidemiologie-france/ressources/glossaire).

Other metadata descriptions were inferred from the metadata editor accessible by authenticated users.



## FichePortailEpidemiologieFrance

| tag                         | description                                           | detail                       |
| --------------------------- | ----------------------------------------------------- | ---------------------------- |
| ```<Metadonnees>```         | Internal metadata of the resource in the  PEF catalog | [link](#metadonnees)         |
| ```<General>```             | ....                                                  | [link](#general)             |
| ```<Caracteristiques>```    | ....                                                  | [link](#caracteristiques)    |
| ```<Collecte>```            | ....                                                  | [link](#collecte)            |
| ```<ValorisationEtAcces>``` | ....                                                  | [link](#valorisationetacces) |


### Metadonnees  

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

| tag                                  | description                                                                                                                                                                                                                          | type        | detail                                          |
| ------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ----------- | ----------------------------------------------- |
| ```<Identification>```               | ...                                                                                                                                                                                                                                  | id          | [link](#general---identification)               |
| ```<ThematiquesGenerales>```         | ....                                                                                                                                                                                                                                 | code        | [link](#general---thematiquesgenerales)         |
| ```<ResponsableScientifique>```      | Person(s) assuming scientific responsibility for the database. This person (or persons) agrees to be contacted for any questions related to the database; if necessary, it is recommended to designate an additional contact person. | code        | [link](#general---responsablescientifique)      |
| ```<Collaborations>```               | Participation or non-participation in discussions and work of consortia or projects (e.g., European projects, etc.).                                                                                                                 | date        | [link](#general---collaborations)               |
| ```<Financements>```                 | ....                                                                                                                                                                                                                                 | date        | [link](#general---financements)                 |
| ```<GouvernanceDeLaBaseDeDonnees>``` | ....                                                                                                                                                                                                                                 | categorical | [link](#general---gouvernancedelabasededonnees) |
| ```<ContactSupplementaire>```        | ....                                                                                                                                                                                                                                 | categorical | [link](#general---contactsupplementaire)        |


#### General - Identification
| tag                  | description                                                                                       | type | detail |
| -------------------- | ------------------------------------------------------------------------------------------------- | ---- | ------ |
| ```<NomFR>```        | The full, precise name or title of the database, survey, or project                               | text |        |
| ```<NomEN>```        | The full, precise name or title of the database, survey, or project                               | text |        |
| ```<AcronymeFR>```   | Abbreviation or Acronym                                                                           | text |        |
| ```<AcronymeEN>```   | Abbreviation or Acronym                                                                           | text |        |
| ```<NumeroCnilFR>``` | A unique identification number assigned by organizations such as ID-RCB, EUDRACT, CNIL, CPP, etc  | text |        |
| ```<NumeroCnilEN>``` | A unique identification number assigned by organizations such as ID-RCB, EUDRACT, CNIL, CPP, etc. | text |        |


#### General - ThematiquesGenerales

| tag                                  | description                                                                                                                                                                                 | type                  | detail |
| ------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------- | ------ |
| ```<DomainesDePathologiesFR>```      | ...                                                                                                                                                                                         | ```<value>``` list    |        |
| ```<DomainesDePathologiesEN>```      | ...                                                                                                                                                                                         | ```<value>``` list    |        |
| ```<CovidFR>```                      | Study related to Covid-19                                                                                                                                                                   | categorical (Oui/Non) |        |
| ```<CovidEN>```                      | ...                                                                                                                                                                                         | categorical (Yes/No)  |        |
| ```<PathologiesFR>```                | Study related to Covid-19                                                                                                                                                                   | text                  |        |
| ```<PathologiesEN>```                | ...                                                                                                                                                                                         | text                  |        |
| ```<DeterminantsDeSanteFR>```        | ...                                                                                                                                                                                         | ```<value>``` list    |        |
| ```<DeterminantsDeSanteEN>```        | ...                                                                                                                                                                                         | ```<value>``` list    |        |
| ```<DomainesMedicauxPrecisionsFR>``` | ...                                                                                                                                                                                         | text                  |        |
| ```<DomainesMedicauxPrecisionsEN>``` | ...                                                                                                                                                                                         | text                  |        |
| ``` <MotsClesFR>```                  | Words or expressions that have particular importance for the indexing and characterization of the database or survey. Keywords help improve the positioning and visibility of the database. | ```<value>``` list    |        |
| ``` <MotsClesEN>```                  | Words or expressions that have particular importance for the indexing and characterization of the database or survey. Keywords help improve the positioning and visibility of the database. | ```<value>``` list    |        |


#### General - ResponsableScientifique

Person(s) assuming scientific responsibility for the database. This person (or persons) agrees to be contacted for any questions related to the database; if necessary, it is recommended to designate an additional contact person.

| tag                                | description | type               | detail |
| ---------------------------------- | ----------- | ------------------ | ------ |
| ``` <ResponsableScientifiqueFR>``` | ...         | ```<value>``` list |        |
| ``` <ResponsableScientifiqueEN>``` | ...         | ```<value>``` list |        |


##### General - ResponsableScientifique - ResponsableScientifiqueFR

| tag                             | description                  | type |
| ------------------------------- | ---------------------------- | ---- |
| ``` <NomResponsable>```         | Name of the person in charge | text |
| ``` <PrenomResponsable>```      | Family name                  | text |
| ``` <AdresseResponsable>```     | Address                      | text |
| ``` <TelephoneResponsable>```   | Telephone number             | text |
| ``` <MailResponsable>```        | E-mail                       | text |
| ``` <LaboratoireResponsable>``` | Laboratory name              | text |
| ``` <OrganismeResponsable>```   | Institution name             | text |

##### General - ResponsableScientifique - ResponsableScientifiqueEN

| tag                             | description                  | type |
| ------------------------------- | ---------------------------- | ---- |
| ``` <NomResponsable>```         | Name of the person in charge | text |
| ``` <PrenomResponsable>```      | Family name                  | text |
| ``` <AdresseResponsable>```     | Address                      | text |
| ``` <TelephoneResponsable>```   | Telephone number             | text |
| ``` <MailResponsable>```        | E-mail                       | text |
| ``` <LaboratoireResponsable>``` | Laboratory name              | text |
| ``` <OrganismeResponsable>```   | Institution name             | text |


#### General - Collaborations

Participation à des projets, des réseaux, des consortiums

Names of the relevant projects, networks, consortia.

| tag                                                                                                                  | description                                          | type |
| -------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------- | ---- |
| ``` <PartenariatsEtReseauxFR>```                                                                                     |
| Participation or non-participation in discussions and work of consortia or projects (e.g., European projects, etc.). | categorical (Oui/Non)                                |
| ``` <PartenariatsEtReseauxFR>```                                                                                     |
| Participation or non-participation in discussions and work of consortia or projects (e.g., European projects, etc.). | categorical (Yes/No)                                 |
| ``` <PartenariatsEtReseauxPrecisionsFR>```                                                                           | Names of the relevant projects, networks, consortia. | ?    |
| ``` <PartenariatsEtReseauxPrecisionsEN>```                                                                           | Names of the relevant projects, networks, consortia. | ?    |
| ``` <AutresCollaborationsFR>```                                                                                      | Other collaborations related to the database.                                 | ?    |
| ``` <AutresCollaborationsEN>```                                                                                      | Other collaborations related to the database.                                  | ?    |


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
| ``` <ObjectifDeLaBaseDeDonnees>``` | ...         | tag  |        |
| ``` <TypeDePopulation>```          | ...         | tag  |        |


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

### Collecte

| tag                              | description | type | detail |
| -------------------------------- | ----------- | ---- | ------ |
| ``` <Dates>```                   | ...         | tag  |        |
| ``` <TailleDeLaBaseDeDonnees>``` | ...         | tag  |        |
| ``` <Donnees>```                 | ...         | tag  |        |
| ``` <Modalites>```               | ...         | tag  |        |

#### Collecte - Dates

| tag                            | description | type | detail |
| ------------------------------ | ----------- | ---- | ------ |
| ``` <AnneePremierRecueilFR>``` | ...         | text |        |
| ``` <AnneePremierRecueilEN>``` | ...         | text |        |
| ``` <AnneeDernierRecueilFR>``` | ...         | text |        |
| ``` <AnneeDernierRecueilEN>``` | ...         | text |        |

#### Collecte - TailleDeLaBaseDeDonnees

| tag                         | description | type               | detail |
| --------------------------- | ----------- | ------------------ | ------ |
| ``` <TailleBaseFR>```       | ...         | ```<value>``` list |        |
| ``` <TailleBaseEN>```       | ...         | ```<value>``` list |        |
| ``` <TailleBaseDetailFR>``` | ...         | text               |        |
| ``` <TailleBaseDetailEN>``` | ...         | text               |        |

#### Collecte - Donnees

| tag                                         | description | type               | detail |
| ------------------------------------------- | ----------- | ------------------ | ------ |
| ``` <EnActiviteFR>```                       | ...         | ```<value>``` list |        |
| ``` <EnActiviteEN>```                       | ...         | ```<value>``` list |        |
| ``` <TypeDonneesRecueilliesFR>```           | ...         | ```<value>``` list |        |
| ``` <TypeDonneesRecueilliesEN>```           | ...         | ```<value>``` list |        |
| ``` <DonneesCliniquesFR>```                 | ...         | ```<value>``` list |        |
| ``` <DonneesCliniquesEN>```                 | ...         | ```<value>``` list |        |
| ``` <DonneesCliniquesPrecisionsFR>```       | ...         | ?                  |        |
| ``` <DonneesCliniquesPrecisionsEN>```       | ...         | ?                  |        |
| ``` <DonneesDeclarativesFR>```              | ...         | ```<value>``` list |        |
| ``` <DonneesDeclarativesEN>```              | ...         | ```<value>``` list |        |
| ``` <DonneesDeclarativesPrecisionsFR>```    | ...         | ?                  |        |
| ``` <DonneesDeclarativesPrecisionsEN>```    | ...         | ?                  |        |
| ``` <DonneesParacliniquesPrecisionsFR>```   | ...         | ?                  |        |
| ``` <DonneesParacliniquesPrecisionsEN>```   | ...         | ?                  |        |
| ``` <DonneesBiologiquesPrecisionsFR>```     | ...         | ?                  |        |
| ``` <DonneesBiologiquesPrecisionsEN>```     | ...         | ?                  |        |
| ``` <DonneesAdministrativesPrecisionsFR>``` | ...         | text               |        |
| ``` <DonneesAdministrativesPrecisionsEN>``` | ...         | text               |        |
| ``` <DonneesCoutPrecisionsFR>```            | ...         | ?                  |        |
| ``` <DonneesCoutPrecisionsEN>```            | ...         | ?                  |        |
| ``` <DonneesUtilitePrecisionsFR>```         | ...         | ?                  |        |
| ``` <DonneesUtilitePrecisionsEN>```         | ...         | ?                  |        |
| ``` <BiothequeFR>```                        | ...         | text               |        |
| ``` <BiothequeEN>```                        | ...         | text               |        |
| ``` <ContenuBiothequeFR>```                 | ...         | ```<value>``` list |        |
| ``` <ContenuBiothequeEN>```                 | ...         | ```<value>``` list |        |
| ``` <BiothequePrecisionsFR>```              | ...         | ?                  |        |
| ``` <BiothequePrecisionsEN>```              | ...         | ?                  |        |
| ``` <ParametreDeSanteFR>```                 | ...         | ```<value>``` list |        |
| ``` <ParametreDeSanteEN>```                 | ...         | ```<value>``` list |        |
| ``` <ConsommationDeSoinsFR>```              | ...         | ```<value>``` list |        |
| ``` <ConsommationDeSoinsEN>```              | ...         | ```<value>``` list |        |
| ``` <QualiteDeVieSantePercueFR>```          | ...         | ?                  |        |
| ``` <QualiteDeVieSantePercueEN>```          | ...         | ?                  |        |
| ``` <AutreParametreObserveFR>```            | ...         | ?                  |        |
| ``` <AutreParametreObserveEN>```            | ...         | ?                  |        |

#### Collecte - Modalites

| tag                                         | description | type                  | detail |
| ------------------------------------------- | ----------- | --------------------- | ------ |
| ``` <ModalitesDeRecueilFR>```               | ...         | text                  |        |
| ``` <ModalitesDeRecueilEN>```               | ...         | text                  |        |
| ``` <NomenclatureFR>```                     | ...         | ?                     |        |
| ``` <NomenclatureEN>```                     | ...         | ?                     |        |
| ``` <ProcedureQualiteFR>```                 | ...         | ?                     |        |
| ``` <ProcedureQualiteEN>```                 | ...         | ?                     |        |
| ``` <SuiviDesParticipantsFR>```             | ...         | categorical (Oui/Non) |        |
| ``` <SuiviDesParticipantsEN>```             | ...         | categorical (Yes/No)  |        |
| ``` <SuiviDesParticipantsModalitesFR>```    | ...         | ```<value>``` list    |        |
| ``` <SuiviDesParticipantsModalitesEN>```    | ...         | ```<value>``` list    |        |
| ``` <DetailDuSuiviFR>```                    | ...         | ?                     |        |
| ``` <DetailDuSuiviEN>```                    | ...         | ?                     |        |
| ``` <SuiviDesParticipantsCimFR>```          | ...         | ?                     |        |
| ``` <SuiviDesParticipantsCimEN>```          | ...         | ?                     |        |
| ``` <SourcesAdministrativesFR>```           | ...         | categorical (Oui/Non) |        |
| ``` <SourcesAdministrativesEN>```           | ...         | categorical (Yes/No)  |        |
| ``` <SourcesAdministrativesPrecisionsFR>``` | ...         | text                  |        |
| ``` <SourcesAdministrativesPrecisionsEN>``` | ...         | text                  |        |

