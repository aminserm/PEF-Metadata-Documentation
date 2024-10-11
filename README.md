# Portail Epidemiologie France (PEF) - XML Export Documentation

This document provides a detailed description of the XML metadata export of the [Portail Epidemiologie France (PEF) catalog](https://epidemiologie-france.aviesan.fr/epidemiologie-france/catalogue).

PEF website provides a glossary of the different metadata sections, in french: [epidemiologie-france.aviesan.fr/epidemiologie-france/ressources/glossaire](https://epidemiologie-france.aviesan.fr/epidemiologie-france/ressources/glossaire).

Other metadata descriptions were inferred from the metadata editor accessible by authenticated users.



## FichePortailEpidemiologieFrance

| tag                         | description                                           | detail                       |
| --------------------------- | ----------------------------------------------------- | ---------------------------- |
| ```<Metadonnees>```         | Internal metadata of the resource in the  PEF catalog | [link](#metadonnees)         |
| ```<General>```             | General                                               | [link](#general)             |
| ```<Caracteristiques>```    | Caracteristiques                                      | [link](#caracteristiques)    |
| ```<Collecte>```            | Collecte                                              | [link](#collecte)            |
| ```<ValorisationEtAcces>``` | Valorisation et accès                                 | [link](#valorisationetacces) |


### Metadonnees  

| tag                                 | description                                | type        |
| ----------------------------------- | ------------------------------------------ | ----------- |
| ```<ID>```                          | ID of the reference within the PEF catalog | id          |
| ```<VersionFR>```                   | Version de la fiche                        | code        |
| ```<VersionEN>```                   | ....                                       | code        |
| ```<DateCreationFicheFR>```         | Date creation de la fiche                  | date        |
| ```<DateCreationFicheEN>```         | ....                                       | date        |
| ```<StatutFicheFR>```               | Statut de la fiche                         | categorical |
| ```<StatutFicheEN>```               | ....                                       | categorical |
| ```<DateChangementStatutFicheFR>``` | Date changement statut de la fiche         | date        |
| ```<DateChangementStatutFicheEN>``` | ....                                       | date        |
| ```<Auteur>```                      | Auteur de la fiche                         | text        |
| ```<UrlFicheFR>```                  | Url de la fiche                            | url         |
| ```<UrlFicheEN>```                  | ....                                       | url         |
| ```<UrlXml>```                      | Url de téléchargement de la fiche XML      | url         |



### General

| tag                                  | description                                                                                                                                                                                                                          | type | detail                                          |
| ------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---- | ----------------------------------------------- |
| ```<Identification>```               | Identification                                                                                                                                                                                                                       | tag  | [link](#general---identification)               |
| ```<ThematiquesGenerales>```         | Thématiques générales                                                                                                                                                                                                                | tag  | [link](#general---thematiquesgenerales)         |
| ```<ResponsableScientifique>```      | Person(s) assuming scientific responsibility for the database. This person (or persons) agrees to be contacted for any questions related to the database; if necessary, it is recommended to designate an additional contact person. | tag  | [link](#general---responsablescientifique)      |
| ```<Collaborations>```               | Participation or non-participation in discussions and work of consortia or projects (e.g., European projects, etc.).                                                                                                                 | tag  | [link](#general---collaborations)               |
| ```<Financements>```                 | Statut des sources de financement ayant permis de constituer la base de données ainsi que celles contribuant à son maintien et/ou à son développement.                                                                               | tag  | [link](#general---financements)                 |
| ```<GouvernanceDeLaBaseDeDonnees>``` | Gouvernance de la base de données                                                                                                                                                                                                    | tag  | [link](#general---gouvernancedelabasededonnees) |
| ```<ContactSupplementaire>```        | Contact(s) supplémentaire(s)                                                                                                                                                                                                         | tag  | [link](#general---contactsupplementaire)        |


#### General - Identification
| tag                  | description                                                                                       | type |
| -------------------- | ------------------------------------------------------------------------------------------------- | ---- |
| ```<NomFR>```        | The full, precise name or title of the database, survey, or project                               | text |
| ```<NomEN>```        | The full, precise name or title of the database, survey, or project                               | text |
| ```<AcronymeFR>```   | Abbreviation or Acronym                                                                           | text |
| ```<AcronymeEN>```   | Abbreviation or Acronym                                                                           | text |
| ```<NumeroCnilFR>``` | A unique identification number assigned by organizations such as ID-RCB, EUDRACT, CNIL, CPP, etc  | text |
| ```<NumeroCnilEN>``` | A unique identification number assigned by organizations such as ID-RCB, EUDRACT, CNIL, CPP, etc. | text |


#### General - ThematiquesGenerales

| tag                                  | description                                                                                                                                                                                                                                | type                  |
| ------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | --------------------- |
| ```<DomainesDePathologiesFR>```      | Différents domaines médicaux abordés dans la base de données.                                                                                                                                                                              | ```<value>``` list    |
| ```<DomainesDePathologiesEN>```      | Different medical fields addressed in the database.                                                                                                                                                                                        | ```<value>```  list   |
| ```<CovidFR>```                      | Etude en lien avec la Covid-19                                                                                                                                                                                                             | categorical (Oui/Non) |
| ```<CovidEN>```                      | Study related to Covid-19                                                                                                                                                                                                                  | categorical (Yes/No)  |
| ```<PathologiesFR>```                | Nom(s) de la (des) pathologie(s) ou du (des) problème(s) de santé qui sont identifiés dans la base de données                                                                                                                              | text                  |
| ```<PathologiesEN>```                | Name(s) of the pathology(ies) or health problem(s) identified in the database.                                                                                                                                                             | text                  |
| ```<DeterminantsDeSanteFR>```        | Déterminants de santé étudiés dans la base de données.                                                                                                                                                                                     | ```<value>``` list    |
| ```<DeterminantsDeSanteEN>```        | Health determinants studied in the database.                                                                                                                                                                                               | ```<value>``` list    |
| ```<DomainesMedicauxPrecisionsFR>``` | Thématique(s) (domaines médicaux ou déterminants de santé) concernant votre base de données et ne figurant pas dans la liste proposée plus haut.                                                                                           | text                  |
| ```<DomainesMedicauxPrecisionsEN>``` | Theme(s) (medical fields or health determinants) related to your database that are not included in the list provided above.                                                                                                                | text                  |
| ```<MotsClesFR>```                   | Words or expressions that have particular importance for the indexing and characterization of the database or survey. Keywords help improve the positioning and visibility of the database.                                                | ```<value>``` list    |
| ```<MotsClesEN>```                   | Mots ou expressions qui ont une importance particulière pour le référencement et la caractérisation de la base de données ou de l'enquête. Les mots-clés contribuent à améliorer le positionnement et la visibilité de la base de données. | ```<value>``` list    |


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

| tag                             | description            | type               | detail                                                             |
| ------------------------------- | ---------------------- | ------------------ | ------------------------------------------------------------------ |
| ```<ContactSupplementaireFR>``` | Contact supplémentaire | ```<value>``` list | [link](#general---contactsupplementaire---contactsupplementairefr) |
| ```<ContactSupplementaireEN>``` | Additional contact     | ```<value>``` list | [link](#general---contactsupplementaire---contactsupplementaireen) |


##### General - ContactSupplementaire - ContactSupplementaireFR

| tag                           | description    | type |
| ----------------------------- | -------------- | ---- |
| ```<ContactSupplementaire>``` | Nom du contact | text |
| ```<PrenomContact>```         | Prénom         | text |
| ```<AdresseContact>```        | Adresse        | text |
| ```<TelephoneContact>```      | Téléphone      | text |
| ```<MailContact>```           | Email          | text |
| ```<LaboratoireContact>```    | Laboratoire    | text |
| ```<OrganismeContact>```      | Organisme      | text |

##### General - ContactSupplementaire - ContactSupplementaireEN

| tag                           | description    | type |
| ----------------------------- | -------------- | ---- |
| ```<ContactSupplementaire>``` | Nom du contact | text |
| ```<PrenomContact>```         | Prénom         | text |
| ```<AdresseContact>```        | Adresse        | text |
| ```<TelephoneContact>```      | Téléphone      | text |
| ```<MailContact>```           | Email          | text |
| ```<LaboratoireContact>```    | Laboratoire    | text |
| ```<OrganismeContact>```      | Organisme      | text |


### Caracteristiques

| tag                               | description                    | type | detail                                                |
| --------------------------------- | ------------------------------ | ---- | ----------------------------------------------------- |
| ```<TypeDeBaseDeDonnees>```       | Type de base de données        | tag  | [link](#caracteristiques---typedebasededonnees)       |
| ```<ObjectifDeLaBaseDeDonnees>``` | Objectif de la base de données | tag  | [link](#caracteristiques---objectifdelabasededonnees) |
| ```<TypeDePopulation>```          | Type de population             | tag  | [link](#caracteristiques---typedepopulation)          |


#### Caracteristiques - TypeDeBaseDeDonnees
| tag                                       | description                                                                                                | type                  |
| ----------------------------------------- | ---------------------------------------------------------------------------------------------------------- | --------------------- |
| ```<TypeDeBaseFR>```                      | Type de base de données                                                                                    | ```<value>``` list    |
| ```<TypeDeBaseEN>```                      | Type of database                                                                                           | ```<value>``` list    |
| ```<TypeDeBaseAutreFR>```                 | Type de base de données. Autres, préciser                                                                  | text                  |
| ```<TypeDeBaseAutreEN>```                 | Other type of database. Please specify                                                                     | text                  |
| ```<TypeEnqueteFR>```                     | Base de données issues d'enquêtes, précisions                                                              | ```<value>``` list    |
| ```<TypeEnqueteEN>```                     | Database resulting from surveys, details                                                                   | ```<value>``` list    |
| ```<RecrutementParIntermediaireFR>```     | Origine du recrutement des participants                                                                    | ```<value>``` list    |
| ```<RecrutementParIntermediaireEN>```     | Source of participant recruitment                                                                          | ```<value>``` list    |
| ```<BaseOuRegistrePrecisionsFR>```        | Base ou registre, précisions                                                                               | text                  |
| ```<BaseOuRegistrePrecisionsEN>```        | Database or registry, details                                                                              | text                  |
| ```<RecrutementSurBaseFR>```              | Critère de sélection des participants                                                                      | ```<value>``` list    |
| ```<RecrutementSurBaseEN>```              | Criteria for selecting participants                                                                        | ```<value>``` list    |
| ```<EnqueteInterventionnelleFR>```        | Le recrutement dans la base de données s'effectue dans le cadre d'une étude interventionnelle              | categorical (Oui/Non) |
| ```<EnqueteInterventionnelleEN>```        | Recruitment in the database occurs as part of an interventional study                                      | categorical (Yes/No)  |
| ```<InterventionnellePrecisionsFR>```     | Le recrutement dans la base de données s'effectue dans le cadre d'une étude interventionnelle. Précisions. | ```<value>``` list    |
| ```<InterventionnellePrecisionsEN>```     | Recruitment in the database occurs as part of an interventional study. Details.                            | ```<value>``` list    |
| ```<ModaliteConstitutionEchantillonFR>``` | Informations complémentaires concernant la constitution de l'échantillon                                   | text                  |
| ```<ModaliteConstitutionEchantillonEN>``` | Additional information regarding sample constitution                                                       | text                  |


#### Caracteristiques - ObjectifDeLaBaseDeDonnees

| tag                         | description          | type |
| --------------------------- | -------------------- | ---- |
| ```<ObjectifGeneralFR>```   | Objectif principal   | text |
| ```<ObjectifGeneralEN>```   | Main objective       | text |
| ```<CriteresInclusionFR>``` | Critères d'inclusion | text |
| ```<CriteresInclusionEN>``` | Inclusion criteria   | text |


#### Caracteristiques - TypeDePopulation

| tag                                   | description                               | type               | detail                                                         |
| ------------------------------------- | ----------------------------------------- | ------------------ | -------------------------------------------------------------- |
| ```<TranchesAgeFR>```                 | Age                                       | ```<value>``` list |                                                                |
| ```<TranchesAgeEN>```                 | Age                                       | ```<value>``` list |                                                                |
| ```<PopulationFR>```                  | Population concernée                      | ```<value>``` list |                                                                |
| ```<PopulationEN>```                  | Target population                         | ```<value>``` list |                                                                |
| ```<PopulationCimFR>```               | Pathologie                                | ```<value>``` list | [link](#caracteristiques---typedepopulation---populationcimfr) |
| ```<PopulationCimEN>```               | Pathology                                 | ```<value>``` list | [link](#caracteristiques---typedepopulation---populationcimen) |
| ```<SexeFR>```                        | Sexe                                      | ```<value>``` list |                                                                |
| ```<SexeEN>```                        | Gender                                    | ```<value>``` list |                                                                |
| ```<ChampGeographiqueFR>```           | Champ géographique                        | ```<value>``` list |                                                                |
| ```<ChampGeographiqueEN>```           | Geographical area                         | ```<value>``` list |                                                                |
| ```<RegionsConcerneesFR>```           | Régions concernées par la base de données | ```<value>``` list |                                                                |
| ```<RegionsConcerneesEN>```           | Regions covered by the database           | ```<value>``` list |                                                                |
| ```<ChampGeographiquePrecisionsFR>``` | Détail du champ géographique              | text               |                                                                |
| ```<ChampGeographiquePrecisionsEN>``` | Geographical area details                 | text               |                                                                |


##### Caracteristiques - TypeDePopulation - PopulationCimFR

| tag         | description                                                            | type |
| ----------- | ---------------------------------------------------------------------- | ---- |
| ```<Cim>``` | Code CIM - Classification internationale des Maladies - CIM 10 GM 2012 | text |

##### Caracteristiques - TypeDePopulation - PopulationCimEN

| tag         | description                                                            | type |
| ----------- | ---------------------------------------------------------------------- | ---- |
| ```<Cim>``` | Code CIM - Classification internationale des Maladies - CIM 10 GM 2012 | text |

### Collecte

| tag                             | description | type | detail                                      |
| ------------------------------- | ----------- | ---- | ------------------------------------------- |
| ```<Dates>```                   | Dates       | tag  | [link](#collecte---dates)                   |
| ```<TailleDeLaBaseDeDonnees>``` | ...         | tag  | [link](#collecte---tailledelabasededonnees) |
| ```<Donnees>```                 | ...         | tag  | [link](#collecte---dates)                   |
| ```<Modalites>```               | ...         | tag  | [link](#collecte---modalites)               |

#### Collecte - Dates

| tag                           | description                  | type |
| ----------------------------- | ---------------------------- | ---- |
| ```<AnneePremierRecueilFR>``` | Année du premier recueil     | text |
| ```<AnneePremierRecueilEN>``` | Year of the first collection | text |
| ```<AnneeDernierRecueilFR>``` | Année du dernier recueil     | text |
| ```<AnneeDernierRecueilEN>``` | Year of the last collection  | text |


#### Collecte - TailleDeLaBaseDeDonnees

| tag                        | description                                          | type               |
| -------------------------- | ---------------------------------------------------- | ------------------ |
| ```<TailleBaseFR>```       | Taille de la base de données (en nombre d'individus) | ```<value>``` list |
| ```<TailleBaseEN>```       | Size of the database (in number of individuals)      | ```<value>``` list |
| ```<TailleBaseDetailFR>``` | Détail du nombre d'individus                         | text               |
| ```<TailleBaseDetailEN>``` | Detail of the number of individuals                  | text               |


#### Collecte - Donnees

| tag                                        | description                                 | type                  |
| ------------------------------------------ | ------------------------------------------- | --------------------- |
| ```<EnActiviteFR>```                       | Activité de la base                         | ```<value>``` list    |
| ```<EnActiviteEN>```                       | Database activity                           | ```<value>``` list    |
| ```<TypeDonneesRecueilliesFR>```           | Type de données recueillies                 | ```<value>``` list    |
| ```<TypeDonneesRecueilliesEN>```           | Type of data collected                      | ```<value>``` list    |
| ```<DonneesCliniquesFR>```                 | Données cliniques, précisions               | ```<value>``` list    |
| ```<DonneesCliniquesEN>```                 | Clinical data, details                      | ```<value>``` list    |
| ```<DonneesCliniquesPrecisionsFR>```       | Détail des données cliniques recueillies    | text                  |
| ```<DonneesCliniquesPrecisionsEN>```       | Details of collected clinical data          | text                  |
| ```<DonneesDeclarativesFR>```              | Données déclaratives, précisions            | ```<value>``` list    |
| ```<DonneesDeclarativesEN>```              | Declarative data, details                   | ```<value>``` list    |
| ```<DonneesDeclarativesPrecisionsFR>```    | Détail des données déclaratives recueillies | text                  |
| ```<DonneesDeclarativesPrecisionsEN>```    | Details of collected declarative data       | text                  |
| ```<DonneesParacliniquesPrecisionsFR>```   | Données paracliniques, précisions           | text                  |
| ```<DonneesParacliniquesPrecisionsEN>```   | Paraclinical data, details                  | text                  |
| ```<DonneesBiologiquesPrecisionsFR>```     | Données biologiques, précisions             | text                  |
| ```<DonneesBiologiquesPrecisionsEN>```     | Biological data, details                    | text                  |
| ```<DonneesAdministrativesPrecisionsFR>``` | Données administratives, précisions         | text                  |
| ```<DonneesAdministrativesPrecisionsEN>``` | Administrative data, details                | text                  |
| ```<DonneesCoutPrecisionsFR>```            | Données de coût, précisions                 | text                  |
| ```<DonneesCoutPrecisionsEN>```            | Cost data, details                          | text                  |
| ```<DonneesUtilitePrecisionsFR>```         | Données d’utilité / préférence, précisions  | text                  |
| ```<DonneesUtilitePrecisionsEN>```         | Utility / preference data, details          | text                  |
| ```<BiothequeFR>```                        | Existence d’une biothèque                   | categorical (Oui/Non) |
| ```<BiothequeEN>```                        | Existence of a biobank                      | categorical (Yes/No)  |
| ```<ContenuBiothequeFR>```                 | Contenu de la biothèque                     | ```<value>``` list    |
| ```<ContenuBiothequeEN>```                 | Content of the biobank                      | ```<value>``` list    |
| ```<BiothequePrecisionsFR>```              | Détail des éléments conservés               | text                  |
| ```<BiothequePrecisionsEN>```              | Details of preserved elements               | text                  |
| ```<ParametreDeSanteFR>```                 | Paramètres de santé étudiés                 | ```<value>``` list    |
| ```<ParametreDeSanteEN>```                 | Health parameters studied                   | ```<value>``` list    |
| ```<ConsommationDeSoinsFR>```              | Consommation de soins, précisions           | ```<value>``` list    |
| ```<ConsommationDeSoinsEN>```              | Healthcare consumption, details             | ```<value>``` list    |
| ```<QualiteDeVieSantePercueFR>```          | Qualité de vie/santé perçue, précisions     | text                  |
| ```<QualiteDeVieSantePercueEN>```          | Perceived quality of life/health, details   | text                  |
| ```<AutreParametreObserveFR>```            | Autres, précisions                          | text                  |
| ```<AutreParametreObserveEN>```            | Others, details                             | text                  |


#### Collecte - Modalites

| tag                                        | complete name                                 | type                  |
| ------------------------------------------ | --------------------------------------------- | --------------------- |
| ```<ModalitesDeRecueilFR>```               | Mode de recueil des données                   | text                  |
| ```<ModalitesDeRecueilEN>```               | Data collection method                        | text                  |
| ```<NomenclatureFR>```                     | Nomenclatures employées                       | text                  |
| ```<NomenclatureEN>```                     | Used nomenclatures                            | text                  |
| ```<ProcedureQualiteFR>```                 | Procédures qualité utilisées                  | text                  |
| ```<ProcedureQualiteEN>```                 | Quality procedures used                       | text                  |
| ```<SuiviDesParticipantsFR>```             | Suivi des participants                        | categorical (Oui/Non) |
| ```<SuiviDesParticipantsEN>```             | Follow-up of participants                     | categorical (Yes/No)  |
| ```<SuiviDesParticipantsModalitesFR>```    | Modalités de suivi des participants           | ```<value>``` list    |
| ```<SuiviDesParticipantsModalitesEN>```    | Follow-up modalities for participants         | ```<value>``` list    |
| ```<DetailDuSuiviFR>```                    | Détail du suivi                               | text                  |
| ```<DetailDuSuiviEN>```                    | Follow-up details                             | text                  |
| ```<SuiviDesParticipantsCimFR>```          | Pathologie suivies                            | ```<value>``` list    |
| ```<SuiviDesParticipantsCimEN>```          | Pathologies followed                          | ```<value>``` list    |
| ```<SourcesAdministrativesFR>```           | Appariement avec des sources administratives  | categorical (Oui/Non) |
| ```<SourcesAdministrativesEN>```           | Matching with administrative sources          | categorical (Yes/No)  |
| ```<SourcesAdministrativesPrecisionsFR>``` | Sources administratives appariées, précisions | text                  |
| ```<SourcesAdministrativesPrecisionsEN>``` | Matched administrative sources, details       | text                  |


### ValorisationEtAcces

| tag                         | description           | type | detail                                             |
| --------------------------- | --------------------- | ---- | -------------------------------------------------- |
| ```<ValorisationEtAcces>``` | Valorisation et accès | tag  | [link](#valorisationetacces---valorisationetacces) |
| ```<Acces>```               | Accès                 | tag  | [link](#valorisationetacces---acces)               |

#### ValorisationEtAcces - ValorisationEtAcces

| tag                         | description                                           | type               | detail                                                             |
| --------------------------- | ----------------------------------------------------- | ------------------ | ------------------------------------------------------------------ |
| ```<PieceJointeFR>```       | Liste des publications relatives à la base de données | ```<value>``` list | [link](#valorisationetacces---valorisationetacces---piecejointefr) |
| ```<PieceJointeEN>```       | List of publications related to the database          | ```<value>``` list | [link](#valorisationetacces---valorisationetacces---piecejointeen) |
| ```<AutreValorisationFR>``` | Autres informations                                   | text               |                                                                    |
| ```<AutreValorisationEN>``` | Other information                                     | text               |                                                                    |

##### ValorisationEtAcces - ValorisationEtAcces - PieceJointeFR

| tag                 | description           | type |
| ------------------- | --------------------- | ---- |
| ```<Fichier>```     | Lien vers le document | text |
| ```<Description>``` | Description           | text |

##### ValorisationEtAcces - ValorisationEtAcces - PieceJointeEN

| tag                 | description           | type |
| ------------------- | --------------------- | ---- |
| ```<Fichier>```     | Lien vers le document | text |
| ```<Description>``` | Description           | text |

#### ValorisationEtAcces - Acces

| tag                                 | description                                                                                                      | type |
| ----------------------------------- | ---------------------------------------------------------------------------------------------------------------- | ---- |
| ```<SiteWebFR>```                   | Lien vers le document                                                                                            | text |
| ```<SiteWebEN>```                   | Link to the document                                                                                             | text |
| ```<ExistenceDocumentCodageFR>```   | Existence d’un document qui répertorie les variables et les modalités de codage:                                 | text |
| ```<ExistenceDocumentCodageEN>```   | Existence of a document listing the variables and coding methods                                                 | text |
| ```<ModalitesAccesFR>```            | Charte d'accès aux données (convention de mise à disposition, format de données et délais de mise à disposition) | text |
| ```<ModalitesAccesEN>```            | Data access charter (data availability agreement, data format, and delivery timelines)                           | text |
| ```<AccesDonneesAgregeesFR>```      | Accès aux données agrégées                                                                                       | text |
| ```<AccesDonneesAgregeesEN>```      | Access to aggregated data                                                                                        | text |
| ```<AccesDonneesIndividuellesFR>``` | Accès aux données individuelles                                                                                  | text |
| ```<AccesDonneesIndividuellesEN>``` | Access to individual data                                                                                        | text |
