# Minimal makefile for Sphinx documentation
#

# You can set these variables from the command line, and also
# from the environment for the first two.
SPHINXOPTS    ?=
SPHINXBUILD   ?= sphinx-build
PUBLISHDIR ?= www_onisep/languages/loms/1.0.0/doc
PUBLISHHOST ?= lheo@boreon.silbercafe.net

SOURCEDIR     = source
BUILDDIR      = build

#
# Doc generation from XSD schemas
#
XSLTPROC ?= xsltproc
TORST = ../../gelaba/xsd-scripts/xsd2rst.xsl
XSDINFO = ../../gelaba/xsd-scripts/xsdlib.xsl
LOMS = ../src/1.0.0/loms-onisep.xsd

# generated with xsltproc --stringparam part targets ../../gelaba/xsd-scripts/xsd2makefile.xsl ../ploteus/static/schemas/LOMSv1.0/loms.xsd
LOMSDOC = source/loms/learningopportunitiesroot.rst \
source/loms/learningopportunityreferences.rst \
source/loms/learningspecificationreferences.rst \
source/loms/learningoutcomereferences.rst \
source/loms/learningoutcomes.rst \
source/loms/learningactivityspecificationreferences.rst \
source/loms/assessmentspecificationreferences.rst \
source/loms/entitlementspecificationreferences.rst \
source/loms/agentreferences.rst \
source/loms/scoringschemereferences.rst \
source/loms/frameworkreferences.rst \
source/loms/learningopportunity.rst \
source/loms/identifier.rst \
source/loms/languagestring.rst \
source/loms/note.rst \
source/loms/document.rst \
source/loms/code.rst \
source/loms/languagecode.rst \
source/loms/uribasedcode.rst \
source/loms/text.rst \
source/loms/languagecharcodeenum.rst \
source/loms/textcontenttypecodeenum.rst \
source/loms/id.rst \
source/loms/documenturl.rst \
source/loms/mailtouri.rst \
source/loms/locationcodecontent.rst \
source/loms/mdrcountrycodeenum.rst \
source/loms/nutscodeenum.rst \
source/loms/languageenum.rst \
source/loms/mdrlanguagecodeenum.rst \
source/loms/idreference.rst \
source/loms/mdrcurrencyenum.rst \
source/loms/iscedfoetcodeenum.rst \
source/loms/eqflevelenum.rst \
source/loms/qualificationframeworkenum.rst \
source/loms/subjecttypecodeenum.rst \
source/loms/escoorganizationtypeenum.rst \
source/loms/reusabilitylevelenum.rst \
source/loms/learningoutcometypeenum.rst \
source/loms/mdradministrativeterritorialunitcodeenum.rst \
source/loms/activitytypeenum.rst \
source/loms/learningopportunitytypeenum.rst \
source/loms/learningmodetypeenum.rst \
source/loms/learningscheduletypeenum.rst \
source/loms/learningsettingtypeenum.rst \
source/loms/targetgroupcodeenum.rst \
source/loms/assessmenttypeenum.rst \
source/loms/entitlementtypeenum.rst \
source/loms/entitlementstatusenum.rst \
source/loms/mediatypeenum.rst \
source/loms/imagemediatypeenum.rst \
source/loms/contentencodingenum.rst \
source/loms/creditpointsystemenum.rst \
source/loms/ectscreditpointsystemenum.rst \
source/loms/skillalignmenttypeenum.rst \
source/loms/currencyenum.rst \
source/loms/mdradministrativeterritorialunitcodecontent.rst \
source/loms/countrycodecontent.rst \
source/loms/legalidentifier.rst \
source/loms/numericscore.rst \
source/loms/creditpoints.rst \
source/loms/ectscreditpoints.rst \
source/loms/amount.rst \
source/loms/locationcode.rst \
source/loms/countrycode.rst \
source/loms/iscedfoetcode.rst \
source/loms/eqflevel.rst \
source/loms/learningoutcometype.rst \
source/loms/reusabilitylevel.rst \
source/loms/learningsettingtype.rst \
source/loms/learningmode.rst \
source/loms/activitytype.rst \
source/loms/targetgroupcode.rst \
source/loms/assessmenttype.rst \
source/loms/learningscheduletype.rst \
source/loms/escoorganizationtype.rst \
source/loms/entitlementtype.rst \
source/loms/entitlementstatus.rst \
source/loms/subjecttypecode.rst \
source/loms/mediatype.rst \
source/loms/imagemediatype.rst \
source/loms/contentencoding.rst \
source/loms/jurisdictioncodecontent.rst \
source/loms/scoringscheme.rst \
source/loms/location.rst \
source/loms/spatialcodelocation.rst \
source/loms/address.rst \
source/loms/phone.rst \
source/loms/mbox.rst \
source/loms/interactivewebresource.rst \
source/loms/mediaobject.rst \
source/loms/imageobject.rst \
source/loms/contactpoint.rst \
source/loms/organization.rst \
source/loms/semanticframework.rst \
source/loms/learningopportunitytype.rst \
source/loms/learningactivityspecification.rst \
source/loms/assessmentspecification.rst \
source/loms/learningspecification.rst \
source/loms/qualification.rst \
source/loms/learningoutcome.rst \
source/loms/awardingopportunity.rst \
source/loms/entitlementspecification.rst \
source/loms/pricedetails.rst \
source/loms/references.rst \
source/loms/gradingscheme.rst \
source/loms/awardingopportunities.rst \
source/loms/haseducationsubject.rst \
source/loms/haseducationlevel.rst \
source/loms/nqflevel.rst \
source/loms/qualificationcode.rst \
source/loms/relatedescoskill.rst \
source/loms/limitoccupation.rst \
source/loms/limitnationaloccupation.rst

# Generated with: xsltproc ../../gelaba/xsd-scripts/xsd2makefile.xsl ../ploteus/static/schemas/LOMSv1.0/loms.xsd
#source/loms/qmslearningopportunities.rst: $(TORST) $(LOMS)
#	$(XSLTPROC) -o $@ --stringparam typename qmsLearningOpportunities $(TORST) $(LOMS)
source/loms/learningopportunitiesroot.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename LearningOpportunitiesRootType $(TORST) $(LOMS)	
source/loms/languagestring.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename LanguageStringType $(TORST) $(LOMS)
source/loms/text.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename TextType $(TORST) $(LOMS)
source/loms/identifier.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename IdentifierType $(TORST) $(LOMS)
source/loms/legalidentifier.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename LegalIdentifierType $(TORST) $(LOMS)
source/loms/numericscore.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename NumericScoreType $(TORST) $(LOMS)
source/loms/creditpoints.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename CreditPointsType $(TORST) $(LOMS)
source/loms/ectscreditpoints.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename ECTSCreditPointsType $(TORST) $(LOMS)
source/loms/amount.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename AmountType $(TORST) $(LOMS)
source/loms/idreference.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename IdReferenceType $(TORST) $(LOMS)
source/loms/note.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename NoteType $(TORST) $(LOMS)
source/loms/code.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename CodeType $(TORST) $(LOMS)
source/loms/uribasedcode.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename URIBasedCodeType $(TORST) $(LOMS)
source/loms/locationcode.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename LocationCodeType $(TORST) $(LOMS)
source/loms/countrycode.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename CountryCodeType $(TORST) $(LOMS)
source/loms/iscedfoetcode.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename IscedFOetCodeType $(TORST) $(LOMS)
source/loms/eqflevel.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename EQFLevelType $(TORST) $(LOMS)
source/loms/learningoutcometype.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename LearningOutcomeTypeType $(TORST) $(LOMS)
source/loms/reusabilitylevel.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename ReusabilityLevelType $(TORST) $(LOMS)
source/loms/learningsettingtype.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename LearningSettingTypeType $(TORST) $(LOMS)
source/loms/learningmode.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename LearningModeType $(TORST) $(LOMS)
source/loms/activitytype.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename ActivityTypeType $(TORST) $(LOMS)
source/loms/learningopportunitytype.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename LearningOpportunityTypeType $(TORST) $(LOMS)
source/loms/targetgroupcode.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename TargetGroupCodeType $(TORST) $(LOMS)
source/loms/assessmenttype.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename AssessmentTypeType $(TORST) $(LOMS)
source/loms/learningscheduletype.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename LearningScheduleTypeType $(TORST) $(LOMS)
source/loms/escoorganizationtype.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename EscoOrganizationTypeType $(TORST) $(LOMS)
source/loms/entitlementtype.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename EntitlementTypeType $(TORST) $(LOMS)
source/loms/entitlementstatus.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename EntitlementStatusType $(TORST) $(LOMS)
source/loms/languagecode.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename LanguageCodeType $(TORST) $(LOMS)
source/loms/subjecttypecode.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename SubjectTypeCodeType $(TORST) $(LOMS)
source/loms/mediatype.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename MediaTypeType $(TORST) $(LOMS)
source/loms/imagemediatype.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename ImageMediaTypeType $(TORST) $(LOMS)
source/loms/contentencoding.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename ContentEncodingType $(TORST) $(LOMS)
source/loms/jurisdictioncodecontent.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename JurisdictionCodeContentType $(TORST) $(LOMS)
source/loms/scoringscheme.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename ScoringSchemeType $(TORST) $(LOMS)
source/loms/document.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename DocumentType $(TORST) $(LOMS)
source/loms/location.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename LocationType $(TORST) $(LOMS)
source/loms/spatialcodelocation.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename SpatialCodeLocationType $(TORST) $(LOMS)
source/loms/address.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename AddressType $(TORST) $(LOMS)
source/loms/phone.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename PhoneType $(TORST) $(LOMS)
source/loms/mbox.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename MBoxType $(TORST) $(LOMS)
source/loms/interactivewebresource.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename InteractiveWebResourceType $(TORST) $(LOMS)
source/loms/mediaobject.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename MediaObjectType $(TORST) $(LOMS)
source/loms/imageobject.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename ImageObjectType $(TORST) $(LOMS)
source/loms/contactpoint.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename ContactPointType $(TORST) $(LOMS)
source/loms/organization.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename OrganizationType $(TORST) $(LOMS)
source/loms/semanticframework.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename SemanticFrameworkType $(TORST) $(LOMS)
source/loms/learningopportunity.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename LearningOpportunityType $(TORST) $(LOMS)
source/loms/learningactivityspecification.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename LearningActivitySpecificationType $(TORST) $(LOMS)
source/loms/assessmentspecification.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename AssessmentSpecificationType $(TORST) $(LOMS)
source/loms/learningspecification.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename LearningSpecificationType $(TORST) $(LOMS)
source/loms/qualification.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename QualificationType $(TORST) $(LOMS)
source/loms/learningoutcome.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename LearningOutcomeType $(TORST) $(LOMS)
source/loms/learningoutcomes.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename LearningOutcomesType $(TORST) $(LOMS)
source/loms/awardingopportunity.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename AwardingOpportunityType $(TORST) $(LOMS)
source/loms/entitlementspecification.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename EntitlementSpecificationType $(TORST) $(LOMS)
source/loms/pricedetails.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename PriceDetailsType $(TORST) $(LOMS)
source/loms/learningopportunityreferences.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename LearningOpportunityReferencesType $(TORST) $(LOMS)
source/loms/learningspecificationreferences.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename LearningSpecificationReferencesType $(TORST) $(LOMS)
source/loms/learningoutcomereferences.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename LearningOutcomeReferencesType $(TORST) $(LOMS)
source/loms/learningactivityspecificationreferences.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename LearningActivitySpecificationReferencesType $(TORST) $(LOMS)
source/loms/assessmentspecificationreferences.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename AssessmentSpecificationReferencesType $(TORST) $(LOMS)
source/loms/entitlementspecificationreferences.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename EntitlementSpecificationReferencesType $(TORST) $(LOMS)
source/loms/agentreferences.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename AgentReferencesType $(TORST) $(LOMS)
source/loms/scoringschemereferences.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename ScoringSchemeReferencesType $(TORST) $(LOMS)
source/loms/frameworkreferences.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename FrameworkReferencesType $(TORST) $(LOMS)
source/loms/references.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename ReferencesType $(TORST) $(LOMS)
source/loms/mdrcountrycodeenum.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename MDRCountryCodeEnumType $(TORST) $(LOMS)
source/loms/mdrlanguagecodeenum.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename MDRLanguageCodeEnumType $(TORST) $(LOMS)
source/loms/nutscodeenum.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename NutsCodeEnumType $(TORST) $(LOMS)
source/loms/mdrcurrencyenum.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename MDRCurrencyEnumType $(TORST) $(LOMS)
source/loms/iscedfoetcodeenum.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename IscedFOetCodeEnumType $(TORST) $(LOMS)
source/loms/eqflevelenum.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename EQFLevelEnumType $(TORST) $(LOMS)
source/loms/qualificationframeworkenum.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename QualificationFrameworkEnumType $(TORST) $(LOMS)
source/loms/subjecttypecodeenum.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename SubjectTypeCodeEnumType $(TORST) $(LOMS)
source/loms/escoorganizationtypeenum.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename EscoOrganizationTypeEnumType $(TORST) $(LOMS)
source/loms/reusabilitylevelenum.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename ReusabilityLevelEnumType $(TORST) $(LOMS)
source/loms/learningoutcometypeenum.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename LearningOutcomeTypeEnumType $(TORST) $(LOMS)
source/loms/mdradministrativeterritorialunitcodeenum.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename MDRAdministrativeTerritorialUnitCodeEnumType $(TORST) $(LOMS)
source/loms/activitytypeenum.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename ActivityTypeEnumType $(TORST) $(LOMS)
source/loms/learningopportunitytypeenum.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename LearningOpportunityTypeEnumType $(TORST) $(LOMS)
source/loms/learningmodetypeenum.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename LearningModeTypeEnumType $(TORST) $(LOMS)
source/loms/learningscheduletypeenum.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename LearningScheduleTypeEnumType $(TORST) $(LOMS)
source/loms/learningsettingtypeenum.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename LearningSettingTypeEnumType $(TORST) $(LOMS)
source/loms/targetgroupcodeenum.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename TargetGroupCodeEnumType $(TORST) $(LOMS)
source/loms/assessmenttypeenum.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename AssessmentTypeEnumType $(TORST) $(LOMS)
source/loms/entitlementtypeenum.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename EntitlementTypeEnumType $(TORST) $(LOMS)
source/loms/entitlementstatusenum.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename EntitlementStatusEnumType $(TORST) $(LOMS)
source/loms/mediatypeenum.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename MediaTypeEnumType $(TORST) $(LOMS)
source/loms/imagemediatypeenum.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename ImageMediaTypeEnumType $(TORST) $(LOMS)
source/loms/contentencodingenum.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename ContentEncodingEnumType $(TORST) $(LOMS)
source/loms/creditpointsystemenum.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename CreditPointSystemEnumType $(TORST) $(LOMS)
source/loms/ectscreditpointsystemenum.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename ECTSCreditPointSystemEnumType $(TORST) $(LOMS)
source/loms/skillalignmenttypeenum.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename SkillAlignmentTypeEnumType $(TORST) $(LOMS)
source/loms/currencyenum.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename CurrencyEnumType $(TORST) $(LOMS)
source/loms/locationcodecontent.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename LocationCodeContentType $(TORST) $(LOMS)
source/loms/mdradministrativeterritorialunitcodecontent.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename MDRAdministrativeTerritorialUnitCodeContentType $(TORST) $(LOMS)
source/loms/countrycodecontent.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename CountryCodeContentType $(TORST) $(LOMS)
source/loms/textcontenttypecodeenum.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename TextContentTypeCodeEnumType $(TORST) $(LOMS)
source/loms/languageenum.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename LanguageEnumType $(TORST) $(LOMS)
source/loms/languagecharcodeenum.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename LanguageCharCodeEnumType $(TORST) $(LOMS)
source/loms/id.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename IdType $(TORST) $(LOMS)
source/loms/documenturl.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename DocumentURLType $(TORST) $(LOMS)
source/loms/mailtouri.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename MailToUriType $(TORST) $(LOMS)
source/loms/gradingscheme.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename GradingSchemeType $(TORST) $(LOMS)
source/loms/awardingopportunities.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename AwardingOpportunitiesType $(TORST) $(LOMS)
source/loms/haseducationsubject.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename HasEducationSubjectType $(TORST) $(LOMS)
source/loms/haseducationlevel.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename HasEducationLevelType $(TORST) $(LOMS)
source/loms/nqflevel.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename NqfLevelType $(TORST) $(LOMS)
source/loms/qualificationcode.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename QualificationCodeType $(TORST) $(LOMS)
source/loms/relatedescoskill.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename RelatedEscoSkillType $(TORST) $(LOMS)
source/loms/limitoccupation.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename LimitOccupationType $(TORST) $(LOMS)
source/loms/limitnationaloccupation.rst: $(TORST) $(LOMS)
	$(XSLTPROC) -o $@ --stringparam typename LimitNationalOccupationType $(TORST) $(LOMS)

# Put it first so that "make" without argument is like "make help".
help:
	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)

.PHONY: help Makefile html clean publish xsdinfo

# Catch-all target: route all unknown targets to Sphinx using the new
# "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
html: Makefile $(LOMSDOC)
	$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)

clean: Makefile
	$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)

publish: html
	ssh $(PUBLISHHOST) "mkdir -p $(PUBLISHDIR)"
	rsync --archive --verbose build/html/. $(PUBLISHHOST):$(PUBLISHDIR)

xsdinfo:
	$(XSLTPROC) --stringparam action list-types $(XSDINFO) $(LOMS)
