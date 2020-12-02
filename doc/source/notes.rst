Notes
=====

Sorry, it's in french.

Plusieurs aspects du schéma sont troublants et induisent une irrégularité dans les outils qui pourraient utiliser ce schéma, par exemple pour extraire de la documentation (tout en n'étant pas à proprement parler des erreurs, le schéma est correct):

- Pourquoi ``gradingScheme`` (avec un attribut ``@idref`` de type ``xs:normalizedString``) n'est pas de type ``. IdReferenceType`` (type avec un attribut ``@idref`` de type ``xsd:anyURI``)? 
- Pourquoi ``LearningOutcomes`` défini directement son contenu plutôt que passer par un type tiers ``LearningOutcomesType``?
- Pourquoi ``awardingOpportunities`` défini directement son contenu plutôt que passer par un type tiers ``awardingOpportunitiesType``?
- Pourquoi ne pas avoir créé de types pour ``hasEducationSubject``, ``hasEducationLevel``, ``nqfLevel``, ``qualificationCode``, ``relatedEscoSkill``, ``limitOccupation``, ``limitNationalOccupation``?

Tous les éléments ``xxxxReferences`` devraient s'appeler ``xxxDefinitions``, car ce ne sont pas des références à des éléments existants mais bien des définitions.

Erreur dans la documentation: "An individual (expected) learning outcome of the learning specification/qualification. It MUST refer to an existing 'LearningOutcome'-record in the 'learningSpecificationReferences'-section of this document." Cela devrait être: *LearningOutcomeReferences*.

Des éléments avec le même nom n'ont pas le même type. Ce n'est pas un bon design (par exemple ``learningActivitySpecification``).
