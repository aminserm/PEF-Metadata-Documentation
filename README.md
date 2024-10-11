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

| tag                                  | description                                                                                                                                                                                                                          | type | detail                                          |
| ------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---- | ----------------------------------------------- |
| ```<Identification>```               | ...                                                                                                                                                                                                                                  | tag  | [link](#general---identification)               |
| ```<ThematiquesGenerales>```         | ....                                                                                                                                                                                                                                 | tag  | [link](#general---thematiquesgenerales)         |
| ```<ResponsableScientifique>```      | Person(s) assuming scientific responsibility for the database. This person (or persons) agrees to be contacted for any questions related to the database; if necessary, it is recommended to designate an additional contact person. | tag  | [link](#general---responsablescientifique)      |
| ```<Collaborations>```               | Participation or non-participation in discussions and work of consortia or projects (e.g., European projects, etc.).                                                                                                                 | tag  | [link](#general---collaborations)               |
| ```<Financements>```                 | Statut des sources de financement ayant permis de constituer la base de données ainsi que celles contribuant à son maintien et/ou à son développement.                                                                               | tag  | [link](#general---financements)                 |
| ```<GouvernanceDeLaBaseDeDonnees>``` | ....                                                                                                                                                                                                                                 | tag  | [link](#general---gouvernancedelabasededonnees) |
| ```<ContactSupplementaire>```        | ....                                                                                                                                                                                                                                 | tag  | [link](#general---contactsupplementaire)        |


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

| tag                                  | description                                                                                                                                                                                                                                | type                  | detail |
| ------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | --------------------- | ------ |
| ```<DomainesDePathologiesFR>```      | Différents domaines médicaux abordés dans la base de données.                                                                                                                                                                              | ```<value>``` list    |        |
| ```<DomainesDePathologiesEN>```      | Different medical fields addressed in the database.                                                                                                                                                                                        | ```<value>```  list   |        |
| ```<CovidFR>```                      | Etude en lien avec la Covid-19                                                                                                                                                                                                             | categorical (Oui/Non) |        |
| ```<CovidEN>```                      | Study related to Covid-19                                                                                                                                                                                                                  | categorical (Yes/No)  |        |
| ```<PathologiesFR>```                | Nom(s) de la (des) pathologie(s) ou du (des) problème(s) de santé qui sont identifiés dans la base de données                                                                                                                              | text                  |        |
| ```<PathologiesEN>```                | Name(s) of the pathology(ies) or health problem(s) identified in the database.                                                                                                                                                             | text                  |        |
| ```<DeterminantsDeSanteFR>```        | Déterminants de santé étudiés dans la base de données.                                                                                                                                                                                     | ```<value>``` list    |        |
| ```<DeterminantsDeSanteEN>```        | Health determinants studied in the database.                                                                                                                                                                                               | ```<value>``` list    |        |
| ```<DomainesMedicauxPrecisionsFR>``` | Thématique(s) (domaines médicaux ou déterminants de santé) concernant votre base de données et ne figurant pas dans la liste proposée plus haut.                                                                                           | text                  |        |
| ```<DomainesMedicauxPrecisionsEN>``` | Theme(s) (medical fields or health determinants) related to your database that are not included in the list provided above.                                                                                                                | text                  |        |
| ```<MotsClesFR>```                   | Words or expressions that have particular importance for the indexing and characterization of the database or survey. Keywords help improve the positioning and visibility of the database.                                                | ```<value>``` list    |        |
| ```<MotsClesEN>```                   | Mots ou expressions qui ont une importance particulière pour le référencement et la caractérisation de la base de données ou de l'enquête. Les mots-clés contribuent à améliorer le positionnement et la visibilité de la base de données. | ```<value>``` list    |        |


#### General - ResponsableScientifique


| tag                               | description                                                                                                                                                                                                                          | type               | detail                                                                 |
| --------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------ | ---------------------------------------------------------------------- |
| ```<ResponsableScientifiqueFR>``` | Person(s) assuming scientific responsibility for the database. This person (or persons) agrees to be contacted for any questions related to the database; if necessary, it is recommended to designate an additional contact person. | ```<value>``` list | [link](#general---responsablescientifique---responsablescientifiquefr) |
| ```<ResponsableScientifiqueEN>``` | Person(s) assuming scientific responsibility for the database. This person (or persons) agrees to be contacted for any questions related to the database; if necessary, it is recommended to designate an additional contact person. | ```<value>``` list | [link](#general---responsablescientifique---responsablescientifiqueen) |


##### General - ResponsableScientifique - ResponsableScientifiqueFR

| tag                            | description                  | type |
| ------------------------------ | ---------------------------- | ---- |
| ```<NomResponsable>```         | Name of the person in charge | text |
| ```<PrenomResponsable>```      | Family name                  | text |
| ```<AdresseResponsable>```     | Address                      | text |
| ```<TelephoneResponsable>```   | Telephone number             | text |
| ```<MailResponsable>```        | E-mail                       | text |
| ```<LaboratoireResponsable>``` | Laboratory name              | text |
| ```<OrganismeResponsable>```   | Institution name             | text |

##### General - ResponsableScientifique - ResponsableScientifiqueEN

| tag                            | description                  | type |
| ------------------------------ | ---------------------------- | ---- |
| ```<NomResponsable>```         | Name of the person in charge | text |
| ```<PrenomResponsable>```      | Family name                  | text |
| ```<AdresseResponsable>```     | Address                      | text |
| ```<TelephoneResponsable>```   | Telephone number             | text |
| ```<MailResponsable>```        | E-mail                       | text |
| ```<LaboratoireResponsable>``` | Laboratory name              | text |
| ```<OrganismeResponsable>```   | Institution name             | text |


#### General - Collaborations

| tag                                       | description                                                                                                          | type                  |
| ----------------------------------------- | -------------------------------------------------------------------------------------------------------------------- | --------------------- |
| ```<PartenariatsEtReseauxFR>```           | Participation or non-participation in discussions and work of consortia or projects (e.g., European projects, etc.). | categorical (Oui/Non) |
| ```<PartenariatsEtReseauxFR>```           | Participation or non-participation in discussions and work of consortia or projects (e.g., European projects, etc.). | categorical (Yes/No)  |
| ```<PartenariatsEtReseauxPrecisionsFR>``` | Names of the relevant projects, networks, consortia.                                                                 | text                  |
| ```<PartenariatsEtReseauxPrecisionsEN>``` | Names of the relevant projects, networks, consortia.                                                                 | text                  |
| ```<AutresCollaborationsFR>```            | Other collaborations related to the database.                                                                        | text                  |
| ```<AutresCollaborationsEN>```            | Other collaborations related to the database.                                                                        | text                  |


#### General - Financements

| tag                              | description                                                                                                                          | type                               |
| -------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------ | ---------------------------------- |
| ```<TypeDeFinancementsFR>```     | Status of the funding sources.                                                                                                       | categorical (Public/Privé/Mixte)   |
| ```<TypeDeFinancementsEN>```     | Status of the funding sources.                                                                                                       | categorical (Public/Private/Mixed) |
| ```<FinancementsPrecisionsFR>``` | Funding sources that enabled the establishment of the database, as well as those contributing to its maintenance and/or development. | text                               |
| ```<FinancementsPrecisionsEN>``` | Funding sources that enabled the establishment of the database, as well as those contributing to its maintenance and/or development. | text                               |

#### General - GouvernanceDeLaBaseDeDonnees

| tag                                  | description                                                                                                                                                            | type                  | detail                                                           |
| ------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------- | ---------------------------------------------------------------- |
| ```<OrganisationFR>```               | Nom et statut de l’institution qui est le porteur et le responsable - au sens juridique - de la base de données ainsi que le statut correspondant à cette institution. | ```<value>``` list    | [link](#general---gouvernancedelabasededonnees---organisationfr) |
| ```<OrganisationEN>```               | Name and status of the institution that is the holder and legally responsible for the database, as well as the corresponding status of this institution.               | ```<value>``` list    | [link](#general---gouvernancedelabasededonnees---organisationen) |
| ```<ExistenceDeComiteFR>```          | Existence de comités scientifique ou de pilotage                                                                                                                       | categorical (Oui/Non) |                                                                  |
| ```<ExistenceDeComiteEN>```          | Existence of scientific or steering committees                                                                                                                         | categorical (Yes/No)  |                                                                  |
| ```<LabellisationsEtExpertisesFR>``` | Labellisations et évaluations de la base de données                                                                                                                    | text                  |                                                                  |
| ```<LabellisationsEtExpertisesEN>``` | Labeling and evaluations of the database                                                                                                                               | text                  |                                                                  |

##### General - GouvernanceDeLaBaseDeDonnees - OrganisationFR

| tag                        | description                                 | type                                             |
| -------------------------- | ------------------------------------------- | ------------------------------------------------ |
| ```<Organisation>```       | Organisation(s) responsable(s) ou promoteur | text                                             |
| ```<StatutOrganisation>``` | Statut de l’organisation                    | categorical (Secteur Public/Secteur Privé/Mixte) |

##### General - GouvernanceDeLaBaseDeDonnees - OrganisationEN

| tag                        | description                             | type                                             |
| -------------------------- | --------------------------------------- | ------------------------------------------------ |
| ```<Organisation>```       | Responsible organization(s) or promoter | text                                             |
| ```<StatutOrganisation>``` | Status of the organisation              | categorical (Public Sector/Private Sector/Mixed) |


#### General - ContactSupplementaire

| tag                             | description | type               | detail |
| ------------------------------- | ----------- | ------------------ | ------ |
| ```<ContactSupplementaireFR>``` | ...         | ```<value>``` list |        |
| ```<ContactSupplementaireEN>``` | ...         | ```<value>``` list |        |


##### General - ContactSupplementaire - ContactSupplementaireFR

| tag                           | description | type | detail |
| ----------------------------- | ----------- | ---- | ------ |
| ```<ContactSupplementaire>``` | ...         | ?    |        |
| ```<PrenomContact>```         | ...         | ?    |        |
| ```<AdresseContact>```        | ...         | ?    |        |
| ```<TelephoneContact>```      | ...         | ?    |        |
| ```<MailContact>```           | ...         | ?    |        |
| ```<LaboratoireContact>```    | ...         | ?    |        |
| ```<OrganismeContact>```      | ...         | ?    |        |

##### General - ContactSupplementaire - ContactSupplementaireEN

| tag                           | description | type | detail |
| ----------------------------- | ----------- | ---- | ------ |
| ```<ContactSupplementaire>``` | ...         | ?    |        |
| ```<PrenomContact>```         | ...         | ?    |        |
| ```<AdresseContact>```        | ...         | ?    |        |
| ```<TelephoneContact>```      | ...         | ?    |        |
| ```<MailContact>```           | ...         | ?    |        |
| ```<LaboratoireContact>```    | ...         | ?    |        |
| ```<OrganismeContact>```      | ...         | ?    |        |


### Caracteristiques

| tag                               | description | type | detail |
| --------------------------------- | ----------- | ---- | ------ |
| ```<TypeDeBaseDeDonnees>```       | ...         | tag  |        |
| ```<ObjectifDeLaBaseDeDonnees>``` | ...         | tag  |        |
| ```<TypeDePopulation>```          | ...         | tag  |        |


#### Caracteristiques - TypeDeBaseDeDonnees

| tag                                       | description | type               | detail |
| ----------------------------------------- | ----------- | ------------------ | ------ |
| ```<TypeDeBaseFR>```                      | ...         | ```<value>``` list |        |
| ```<TypeDeBaseEN>```                      | ...         | ```<value>``` list |        |
| ```<TypeDeBaseAutreFR>```                 | ...         | ?                  |        |
| ```<TypeDeBaseAutreEN>```                 | ...         | ?                  |        |
| ```<TypeEnqueteFR>```                     | ...         | ```<value>``` list |        |
| ```<TypeEnqueteEN>```                     | ...         | ```<value>``` list |        |
| ```<RecrutementParIntermediaireFR>```     | ...         | ```<value>``` list |        |
| ```<RecrutementParIntermediaireEN>```     | ...         | ```<value>``` list |        |
| ```<BaseOuRegistrePrecisionsFR>```        | ...         | ?                  |        |
| ```<BaseOuRegistrePrecisionsEN>```        | ...         | ?                  |        |
| ```<RecrutementSurBaseFR>```              | ...         | ```<value>``` list |        |
| ```<RecrutementSurBaseEN>```              | ...         | ```<value>``` list |        |
| ```<EnqueteInterventionnelleFR>```        | ...         | ?                  |        |
| ```<EnqueteInterventionnelleEN>```        | ...         | ?                  |        |
| ```<InterventionnellePrecisionsFR>```     | ...         | ```<value>``` list |        |
| ```<InterventionnellePrecisionsEN>```     | ...         | ```<value>``` list |        |
| ```<ModaliteConstitutionEchantillonFR>``` | ...         | text               |        |
| ```<ModaliteConstitutionEchantillonEN>``` | ...         | text               |        |


#### Caracteristiques - ObjectifDeLaBaseDeDonnees

| tag                         | description | type | detail |
| --------------------------- | ----------- | ---- | ------ |
| ```<ObjectifGeneralFR>```   | ...         | text |        |
| ```<ObjectifGeneralEN>```   | ...         | text |        |
| ```<CriteresInclusionFR>``` | ...         | text |        |
| ```<CriteresInclusionEN>``` | ...         | text |        |

#### Caracteristiques - TypeDePopulation

| tag                                   | description | type               | detail |
| ------------------------------------- | ----------- | ------------------ | ------ |
| ```<TranchesAgeFR>```                 | ...         | ```<value>``` list |        |
| ```<TranchesAgeEN>```                 | ...         | ```<value>``` list |        |
| ```<PopulationFR>```                  | ...         | ```<value>``` list |        |
| ```<PopulationEN>```                  | ...         | ```<value>``` list |        |
| ```<PopulationCimFR>```               | ...         | ```<value>``` list |        |
| ```<PopulationCimEN>```               | ...         | ```<value>``` list |        |
| ```<SexeFR>```                        | ...         | ```<value>``` list |        |
| ```<SexeEN>```                        | ...         | ```<value>``` list |        |
| ```<ChampGeographiqueFR>```           | ...         | ```<value>``` list |        |
| ```<ChampGeographiqueEN>```           | ...         | ```<value>``` list |        |
| ```<RegionsConcerneesFR>```           | ...         | ```<value>``` list |        |
| ```<RegionsConcerneesEN>```           | ...         | ```<value>``` list |        |
| ```<ChampGeographiquePrecisionsFR>``` | ...         | text               |        |
| ```<ChampGeographiquePrecisionsEN>``` | ...         | text               |        |

##### Caracteristiques - TypeDePopulation - PopulationCimFR

| tag         | description | type | detail |
| ----------- | ----------- | ---- | ------ |
| ```<Cim>``` | ...         | text |        |

##### Caracteristiques - TypeDePopulation - PopulationCimEN

| tag         | description | type | detail |
| ----------- | ----------- | ---- | ------ |
| ```<Cim>``` | ...         | text |        |

### Collecte

| tag                             | description | type | detail |
| ------------------------------- | ----------- | ---- | ------ |
| ```<Dates>```                   | ...         | tag  |        |
| ```<TailleDeLaBaseDeDonnees>``` | ...         | tag  |        |
| ```<Donnees>```                 | ...         | tag  |        |
| ```<Modalites>```               | ...         | tag  |        |

#### Collecte - Dates

| tag                           | description | type | detail |
| ----------------------------- | ----------- | ---- | ------ |
| ```<AnneePremierRecueilFR>``` | ...         | text |        |
| ```<AnneePremierRecueilEN>``` | ...         | text |        |
| ```<AnneeDernierRecueilFR>``` | ...         | text |        |
| ```<AnneeDernierRecueilEN>``` | ...         | text |        |

#### Collecte - TailleDeLaBaseDeDonnees

| tag                        | description | type               | detail |
| -------------------------- | ----------- | ------------------ | ------ |
| ```<TailleBaseFR>```       | ...         | ```<value>``` list |        |
| ```<TailleBaseEN>```       | ...         | ```<value>``` list |        |
| ```<TailleBaseDetailFR>``` | ...         | text               |        |
| ```<TailleBaseDetailEN>``` | ...         | text               |        |

#### Collecte - Donnees

| tag                                         | description | type               | detail |
| ------------------------------------------- | ----------- | ------------------ | ------ |
| ```<EnActiviteFR>```                        | ...         | ```<value>``` list |        |
| ```<EnActiviteEN>```                        | ...         | ```<value>``` list |        |
| ```<TypeDonneesRecueilliesFR>```            | ...         | ```<value>``` list |        |
| ```<TypeDonneesRecueilliesEN>```            | ...         | ```<value>``` list |        |
| ```<DonneesCliniquesFR>```                  | ...         | ```<value>``` list |        |
| ```<DonneesCliniquesEN>```                  | ...         | ```<value>``` list |        |
| ```<DonneesCliniquesPrecisionsFR>```        | ...         | ?                  |        |
| ```<DonneesCliniquesPrecisionsEN>```        | ...         | ?                  |        |
| ```<DonneesDeclarativesFR>```               | ...         | ```<value>``` list |        |
| ```<DonneesDeclarativesEN>```               | ...         | ```<value>``` list |        |
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

