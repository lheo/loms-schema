LOMS Document
=============


Example
-------

The following XML extract shows the structure of an XML document that adheres to the LOMS XSD definition.

.. code-block:: xml

  <qmsLearningOpportunities
        xmlns="http://data.europa.eu/europass/qms-xml/schema/learning-opportunities">
    <learningOpportunities> <!-- 1,1 -->
      <learningOpportunity id="...IdType..."> <!-- 0,N -->
        <identifier>...IdentifierType...</identifier> <!-- 1,N -->
        <title>...LanguageStringType...</title> <!-- 1,N -->
        <altLabel>...LanguageStringType...</altLabel> <!-- 0,N -->
        <description>...NoteType...</description> <!-- 0,N -->
        <additionalNote>...NoteType...</additionalNote> <!-- 0,N -->
        <homepage>...DocumentType...</homepage> <!-- 0,N -->
        <supplementaryDoc>...DocumentType...</supplementaryDoc> <!-- 0,N -->
        <startedAtDate>...xs:date...</startedAtDate> <!-- 0,1 -->
        <endedAtDate>...xs:date...</endedAtDate> <!-- 0,1 -->
        <duration>...xs:duration...</duration> <!-- 0,1 -->
        <learningSchedule>...LearningScheduleTypeType...</learningSchedule> <!-- 0,1 -->
        <scheduleInformation>...NoteType...</scheduleInformation> <!-- 0,N -->
        <admissionProcedure>...NoteType...</admissionProcedure> <!-- 0,N -->
        <priceDetails>...PriceDetailsType...</priceDetails> <!-- 0,N -->
        <providedBy>...IdReferenceType(organization)...</providedBy> <!-- 1,N -->
        <providedAt>...LocationType...</providedAt> <!-- 0,N -->
        <specifiedBy> <!-- 1,1 -->
          ...IdReferenceType(learningSpecification|qualification|qualificationRef)...
        </specifiedBy>
        <hasPart>...IdReferenceType(learningOpportunity/@id)...</hasPart> <!-- 0,N -->
        <referenceLanguage>...LanguageCodeType...</referenceLanguage> <!-- 0,1 -->
      </learningOpportunity>
    </learningOpportunities>
    <learningSpecificationReferences> <!-- 0,1 / choice -->
      <learningSpecification id="...IdType..."> <!-- 0,N -->
        <!-- LearningSpecificationElements -->
        <identifier>...IdentifierType...</identifier> <!-- 0,N -->
        <type>...LearningOpportunityTypeType...</type> <!-- 0,N -->
        <title>...LanguageStringType...</title> <!-- 1,N -->
        <altLabel>...LanguageStringType...</altLabel> <!-- 0,N -->
        <definition>...NoteType...</definition> <!-- 0,N -->
        <description>...NoteType...</description> <!-- 0,N -->
        <additionalNote>...NoteType...</additionalNote> <!-- 0,N -->
        <homepage>...DocumentType...</homepage> <!-- 0,N -->
        <supplementaryDoc>...DocumentType...</supplementaryDoc> <!-- 0,N -->
        <hasISCED-FCode>...IscedFOetCodeType...</hasISCED-FCode> <!-- 1,N -->
        <hasEducationSubject>...???...</hasEducationSubject> <!-- 0,N -->
        <volumeOfLearning>...xs:duration...</volumeOfLearning> <!-- 0,1 -->
        <hasECTSCreditPoints>...ECTSCreditPointsType...</hasECTSCreditPoints> <!-- 0,1 -->
        <hasCreditPoints>...CreditPointsType...</hasCreditPoints> <!-- 0,N -->
        <hasEducationLevel>...???...</hasEducationLevel> <!-- 0,N -->
        <language>...LanguageCodeType...</language> <!-- 0,N -->
        <mode>...LearningModeType...</mode> <!-- 0,N -->
        <learningSettingType>....LearningSettingTypeType...</learningSettingType> <!-- 0,1 -->
        <duration>...xs:duration...</duration> <!-- 0,1 -->
        <targetGroup>....TargetGroupCodeType...</targetGroup> <!-- 0,N -->
        <entryRequirementsNote>...NoteType...</entryRequirementsNote> <!-- 0,N -->
        <learningOutcomes> <!-- 1,1 -->
          <learningOutcome> <!-- 1,N -->
            ...IdReferenceType(LearningOutcome/@id)...
          </learningOutcome>
        </learningOutcomes>
        <learningActivitySpecification> <!-- 0,1 -->
            ...IdReferenceType(learningActivitySpecification/@id)...
        </learningActivitySpecification>
        <assessmentSpecification> <!-- 0,1 -->
            ...IdReferenceType(assessmentSpecificationReferences/AssessmentSpecification/@id)...
        </assessmentSpecification>
        <entitlementSpecification> <!-- 0,N -->
            ...IdReferenceType(entitlementSpecificationReferences/entitlementSpecification/@id)...
        </entitlementSpecification>
        <awardingOpportunities> <!-- 0,1 -->
            <awardingOpportunity>...AwardingOpportunityType...</awardingOpportunity> <!-- 0,N -->
        </awardingOpportunities>
        <!-- /LearningSpecificationElements -->
        <hasPart>...IdReferenceType...</hasPart> <!-- 0,N -->
        <specializationOf>...IdReferenceType...</specializationOf> <!-- 0,N -->
      </learningSpecification>
      <qualification id="...IdType..."> <!-- 0,N -->
        <!-- LearningSpecificationElements -->
        <!-- ... see learningSpecification -->
        <!-- /LearningSpecificationElements -->
        <isPartialQualification>...xs:boolean...</isPartialQualification>
        <eqfLevel>...EQFLevelType...</eqfLevel> <!-- 1,1 -->
        <nqfLevel>...???...</nqfLevel> <!-- 1,N -->
        <qualificationCode>...???...</qualificationCode> <!-- 0,N -->
        <hasPart>...IdReferenceType...</hasPart> <!-- 0,N -->
        <specializationOf>...IdReferenceType...</specializationOf> <!-- 0,1 -->
      </qualification>
      <qualificationRef id="...IdType..."> <!-- 0,N -->
        <identifier>...IdentifierType...</identifier> <!-- 1,1 -->
      </qualification>
    </learningSpecificationReferences>
    <learningOutcomeReferences> <!-- 0,1 -->
      <learningOutcome id="...IdType..."> <!-- 1,N -->
        <identifier>...IdentifierType...</identifier> <!-- 0,N -->
        <prefLabel>...LanguageStringType...</prefLabel> <!-- 1,N -->
        <description>...NoteType...</description> <!-- 0,N -->
        <learningOutcomeType>...LearningOutcomeTypeType...</learningOutcomeType> <!-- 0,1 -->
        <reusabilityLevel>...ReusabilityLevelType...</reusabilityLevel> <!-- 0,1 -->
        <relatedEscoSkill>...???...</relatedEscoSkill> <!-- 0,N -->
      </learningOutcome>
    </learningOutcomeReferences>
    <learningActivitySpecificationReferences> <!-- 0,1 -->
      <learningActivitySpecification id="...IdType..."> <!-- 0,N -->
        <!-- CommonSpecificationElements -->
        <identifier>...IdentifierType...</identifier> <!-- 0,N -->
        <title>...LanguageStringType...</title> <!-- 0,N -->
        <altLabel>...LanguageStringType...</altLabel> <!-- 0,N -->
        <description>...NoteType...</description> <!-- 0,N -->
        <additionalNote>...NoteType...</additionalNote> <!-- 0,N -->
        <homepage>...DocumentType...</homepage> <!-- 0,N -->
        <supplementaryDoc>...DocumentType...</supplementaryDoc> <!-- 0,N -->
        <!-- /CommonSpecificationElements -->
        <type>...ActivityTypeType...</type> <!-- 0,N -->
        <workload>...xs:duration...</workload> <!-- 0,1 -->
        <language>...LanguageCodeType...</language> <!-- 0,N -->
        <mode>...LearningModeType...</mode> <!-- 0,N -->
        <teaches>...IdReferenceType...</teaches> <!-- 0,N -->
        <hasPart>...IdReferenceType...</hasPart> <!-- 0,N -->
        <specializationOf>...IdReferenceType...</specializationOf> <!-- 0,N -->
      </learningActivitySpecification>
    </learningActivitySpecificationReferences>
    <assessmentSpecificationReferences> <!-- 0,1 -->
      <assessmentSpecification id="...IdType..."> <!-- 0,N -->
        <!-- CommonSpecificationElements -->
        <identifier>...IdentifierType...</identifier> <!-- 0,N -->
        <title>...LanguageStringType...</title> <!-- 0,N -->
        <altLabel>...LanguageStringType...</altLabel> <!-- 0,N -->
        <description>...NoteType...</description> <!-- 0,N -->
        <additionalNote>...NoteType...</additionalNote> <!-- 0,N -->
        <homepage>...DocumentType...</homepage> <!-- 0,N -->
        <supplementaryDoc>...DocumentType...</supplementaryDoc> <!-- 0,N -->
        <!-- /CommonSpecificationElements -->
        <type>...AssessmentTypeType...</type> <!-- 0,N -->
        <language>...LanguageCodeType...</language> <!-- 0,N -->
        <mode>...LearningModeType...</mode> <!-- 0,N -->
        <gradingScheme idref="...xs:normalizedString..." /> <!-- 0,N -->
        <proves>...IdReferenceType...</proves> <!-- 0,N -->
        <hasPart>...IdReferenceType...</hasPart> <!-- 0,N -->
        <specializationOf>...IdReferenceType...</specializationOf> <!-- 0,N -->
      </assessmentSpecification>
    </assessmentSpecificationReferences>
    <entitlementSpecificationReferences> <!-- 0,1 -->
      <entitlementSpecification id="...IdType..."> <!-- 0,N -->
        <!-- CommonSpecificationElements -->
        <identifier>...IdentifierType...</identifier> <!-- 0,N -->
        <title>...LanguageStringType...</title> <!-- 0,N -->
        <altLabel>...LanguageStringType...</altLabel> <!-- 0,N -->
        <description>...NoteType...</description> <!-- 0,N -->
        <additionalNote>...NoteType...</additionalNote> <!-- 0,N -->
        <homepage>...DocumentType...</homepage> <!-- 0,N -->
        <supplementaryDoc>...DocumentType...</supplementaryDoc> <!-- 0,N -->
        <!-- /CommonSpecificationElements -->
        <type>...EntitlementTypeType...</type> <!-- 1,1 -->
        <status>...EntitlementStatusType...</status> <!-- 1,1 -->
        <limitOrganization>...IdReferenceType...</limitOrganization> <!-- 0,N -->
        <limitJurisdiction>...JurisdictionCodeContentType...</limitJurisdiction> <!-- 0,N -->
        <limitOccupation>...??...</limitOccupation> <!-- 0,N -->
        <limitNationalOccupation>...??...</limitNationalOccupation> <!-- 0,N -->
        <mayResultFrom>...IdReferenceType...</mayResultFrom> <!-- 0,N -->
        <hasPart>...IdReferenceType...</hasPart> <!-- 0,N -->
        <specializationOf>...IdReferenceType...</specializationOf> <!-- 0,N -->
      </entitlementSpecification>
    </entitlementSpecificationReferences>
    <agentReferences> <!-- 0,1 -->
      <organization id="...IdType..."> <!-- 0,N -->
        <registration>...LegalIdentifierType...</registration> <!-- 0,1 -->
        <vatIdentifier>...LegalIdentifierType...</vatIdentifier> <!-- 0,N -->
        <taxIdentifier>...LegalIdentifierType...</taxIdentifier> <!-- 0,N -->
        <identifier>...IdentifierType...</identifier> <!-- 0,N -->
        <type>...EscoOrganizationTypeType...</type> <!-- 0,N -->
        <prefLabel>...LanguageStringType...</prefLabel> <!-- 1,N -->
        <altLabel>...LanguageStringType...</altLabel> <!-- 0,N -->
        <homepage>...DocumentType...</homepage> <!-- 0,N -->
        <additionalNote>...NoteType...</additionalNote> <!-- 0,N -->
        <hasLocation>...SpatialCodeLocationType...</hasLocation> <!-- 1,N -->
        <contactPoint>...ContactPointType...</contactPoint> <!-- 0,N -->
        <hasUnit>...IdReferenceType...</hasUnit> <!-- 0,N -->
        <unitOf>...IdReferenceType...</unitOf> <!-- 0,1 -->
        <logo>...ImageObjectType...</logo> <!-- 0,1 -->
        <lastModificationDate>...xs:dateTime...</lastModificationDate> <!-- 0,1 -->
      </organization>
    </agentReferences>
    <scoringSchemeReferences> <!-- 0,1 -->
      <scoringScheme id="...xs:normalizedString..."> <!-- 0,N -->
        <identifier>...IdentifierType...</identifier> <!-- 0,N -->
        <title>...LanguageStringType...</title> <!-- 1,N -->
        <description>...NoteType...</description> <!-- 0,N -->
        <supplementaryDoc>...DocumentType...</supplementaryDoc> <!-- 0,N -->
      </scoringScheme>
    </scoringSchemeReferences>
    <semanticFrameworkReferences> <!-- 0,1 -->
      <framework id="...IdType..."> <!-- 0,N -->
        <identifier>...IdentifierType...</identifier> <!-- 0,N -->
        <title>...LanguageStringType...</title> <!-- 1,N -->
        <description>...NoteType...</description> <!-- 0,N -->
        <supplementaryDoc>...DocumentType...</supplementaryDoc> <!-- 0,N -->
      </framework>
    </semanticFrameworkReferences>
  </qmsLearningOpportunities>

The smallest documents
----------------------

Following this definition, the smallest possible document looks like this:

.. code-block:: xml

    <qmsLearningOpportunities xmlns="http://data.europa.eu/europass/qms-xml/schema/learning-opportunities">
        <learningOpportunities/>
    </qmsLearningOpportunities>

And if we put some content, the smallest possible document is:

.. code-block:: xml

    <?xml version="1.0"?>
    <qmsLearningOpportunities xmlns="http://data.europa.eu/europass/qms-xml/schema/learning-opportunities">
        <learningOpportunities>
            <learningOpportunity id="urn:1">
                <identifier>urn:1</identifier>
                <title><text lang="fr" content-type="text/plain">Ma formation</text></title>
                <providedBy idref="urn:orga:1"/>
                <specifiedBy idref="urn:forma:1"/>
            </learningOpportunity>
        </learningOpportunities>
        <learningSpecificationReferences>
            <learningSpecification id="urn:forma:1">
                <title><text lang="fr" content-type="text/plain">Contenu de ma formation</text></title>
                <hasISCED-FCode uri="http://data.europa.eu/esco/isced-f/1013"/>
                <learningOutcomes>
                    <learningOutcome idref="urn:outcome:1"/>
                </learningOutcomes>
            </learningSpecification>
        </learningSpecificationReferences>
        <learningOutcomeReferences>
            <learningOutcome id="urn:outcome:1">
                <prefLabel><text lang="fr" content-type="text/plain">CAP Photographe</text></prefLabel>
            </learningOutcome>
        </learningOutcomeReferences>
        <agentReferences>
            <organization id="urn:orga:1">
                <prefLabel><text lang="fr" content-type="text/plain">ONISEP</text></prefLabel>
                <hasLocation>
                    <spatialCode uri="http://publications.europa.eu/resource/authority/country/FRA"/>
                </hasLocation>
            </organization>
        </agentReferences>
    </qmsLearningOpportunities>

