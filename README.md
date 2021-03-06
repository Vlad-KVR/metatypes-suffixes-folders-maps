# Metatypes suffixes (extensions) map. Metatypes folders map. Salesforce
Source: https://developer.salesforce.com/docs/atlas.en-us.api_meta.meta/api_meta/meta_types_list.htm

<p>To use these maps, you need to carefully familiarize yourself with the types marked "not found", "need to be careful" and decide whether to use them. Also, one type may exist in one map, but it may not be in the second.</p>
<p>These maps are written in the Apex language.</p>

<b>Metatypes folders map</b>
<pre>    public static final Map<String, String> metaTypeFolderMap = new Map<String, String> {
            'AccountRelationshipShareRule' => 'accountRelationshipShareRules',
            'ActionLinkGroupTemplate' => 'actionLinkGroupTemplates',
            'ActionPlanTemplate' => 'actionPlanTemplates',
            'AIApplication' => 'aiApplications',
            'AIApplicationConfig' => 'aiApplicationConfigs',
            'AnalyticSnapshot' => 'analyticSnapshots',
            'AnimationRule' => 'animationRules',
            'ArticleType' => 'objects',
            'ApexClass' => 'classes',
            'ApexComponent' => 'components',
            'ApexEmailNotifications' => 'apexEmailNotifications',
            'ApexPage' => 'pages',
            'ApexTestSuite' => 'testSuites',
            'ApexTrigger' => 'triggers',
//            'AppMenu' => '', not found !!!
            'AppointmentAssignmentPolicy' => 'appointmentSchedulingPolicies',
            'AppointmentSchedulingPolicy' => 'appointmentSchedulingPolicies',
            'ApprovalProcess' => 'approvalProcesses',
            'AssignmentRules' => 'assignmentRules',
            'Audience' => 'audience',
            'AuraDefinitionBundle' => 'aura',
            'AuthProvider' => 'authproviders',
            'AutoResponseRules' => 'autoResponseRules',
            'BatchCalcJobDefinition' => 'batchCalcJobDefinitions',
            'BatchProcessJobDefinition' => 'batchProcessJobDefinitions',
            'Bot' => 'bot',
            'BotVersion' => 'bot',
            'BrandingSet' => 'brandingSets',
            'BriefcaseDefinition' => 'briefcaseDefinitions',
            'BusinessProcessGroup' => 'businessProcessGroups',
            'CallCenter' => 'callCenters',
            'CallCoachingMediaProvider' => 'CallCoachingMediaProvider',
            'CampaignInfluenceModel' => 'campaignInfluenceModels',
            'CaseSubjectParticle' => 'CaseSubjectParticles',
            'CareSystemFieldMapping' => 'careSystemFieldMappings',
            'CareProviderSearchConfig' => 'careProviderSearchConfigs',
            'Certificate' => 'certs',
//            'ChatterExtension' => '', not found !!!
            'CleanDataService' => 'cleanDataServices',
            'CMSConnectSource' => 'cmsConnectSource',
            'Community' => 'communities', // In API version 28, the API object label has changed to Zone, but the API type is still Community !!!
            'Zone' => 'communities', // In API version 28, the API object label has changed to Zone, but the API type is still Community !!!
            'CommunityTemplateDefinition' => 'communityTemplateDefinitions',
            'CommunityThemeDefinition' => 'communityThemeDefinitions',
            'ConnectedApp' => 'connectedApps',
            'ContentAsset' => 'contentassets',
            'CorsWhitelistOrigin' => 'corswhitelistorigins',
            'CspTrustedSite' => 'cspTrustedSites',
            'CustomApplication' => 'applications',
            'CustomApplicationComponent' => 'customApplicationComponents',
            'CustomFeedFilter' => 'feedFilters',
            'CustomHelpMenuSection' => 'customHelpMenuSections',
//            'CustomLabels' => '', not found, all custom labels store in 'labels/CustomLabels.labels' !!!
            'CustomMetadata' => 'objects',
            'CustomNotificationType' => 'notificationtypes',
            'CustomObject' => 'objects',
            'CustomObjectTranslation' => 'objectTranslations',
            'CustomPageWebLink' => 'weblinks',
            'CustomPermission' => 'customPermissions',
            'CustomSite' => 'sites',
            'CustomTab' => 'tabs',
//            'CustomValue' => '', not found !!!
            'CustomTab' => 'dashboards',
            'DataCategoryGroup' => 'datacategorygroups',
            'DataCategoryGroup' => 'datacategorygroups',
            'DataPackageKitObject' => 'DataPackageKitObjects',
            'DataConnectorS3' => 's3DataConnectors',
            'DataSource' => 'mktDataSources',
            'DataSourceObject' => 'mktDataSourceObjects',
            'DataStreamDefinition' => 'dataStreamDefinitions',
            'DecisionTable' => 'decisionTables',
            'DecisionTableDatasetLink' => 'decisionTableDatasetLinks',
            'DelegateGroup' => 'delegateGroups',
            'DiscoveryAIModel' => 'discovery',
            'DiscoveryGoal' => 'discovery',
            'Document' => 'DocumentFolder', // need to be careful !!!
            'DuplicateRule' => 'duplicateRules',
            'EclairGeoData' => 'eclair',
            'EmailServicesFunction' => 'emailservices',
            'EmailTemplate' => 'email',
            'EmbeddedServiceBranding' => 'EmbeddedServiceBranding',
            'EmbeddedServiceConfig' => 'EmbeddedServiceConfig',
            'EmbeddedServiceFieldService' => 'EmbeddedServiceFieldService',
            'EmbeddedServiceFlowConfig' => 'EmbeddedServiceFlowConfig',
            'EmbeddedServiceLiveAgent' => 'EmbeddedServiceLiveAgent',
            'EmbeddedServiceMenuSettings' => 'EmbeddedServiceMenuSettings',
            'EntitlementProcess' => 'entitlementProcesses',
            'EntitlementTemplate' => 'entitlementTemplates',
            'EscalationRules' => 'escalationRules',
            'EventDelivery' => 'eventDeliveries',
            'EventSubscription' => 'eventSubscriptions',
//            'ExperienceBundle' => '', not found !!!
            'ExternalDataConnector' => 'externalDataConnectors',
            'ExternalDataSource' => 'dataSources',
            'ExternalServiceRegistration' => 'dataSources',
            'FeatureParameterBoolean' => 'featureParameters',
            'FeatureParameterDate' => 'featureParameters',
            'FeatureParameterInteger' => 'featureParameters',
            'FieldRestrictionRule' => 'fieldRestrictionRules',
            'FieldSrcTrgtRelationship' => 'fieldSrcTrgtRelationship',
            'FlexiPage' => 'flexipages',
            'Flow' => 'Flow',
            'FlowCategory' => 'flowCategories',
            'FlowDefinition' => 'flowDefinitions',
//            'Folder' => '', can be documents, email, reports, and dashboards !!!
            'ForecastingSourceDefinition' => 'forecastingSourceDefinitions',
            'ForecastingType' => 'forecastingTypes',
            'ForecastingTypeSource' => 'ForecastingTypeSources',
            'FunctionReference' => 'functions',
//            'GatewayProviderPaymentMethodType' => '', not found !!!
            'GlobalPicklist' => 'globalPicklist',
//            'GlobalPicklistValue' => '', not found !!!
            'GlobalValueSet' => 'globalValueSets',
            'GlobalValueSetTranslation' => 'globalValueSetTranslations',
            'Group' => 'groups',
            'HomePageComponent' => 'homepagecomponents',
            'HomePageLayout' => 'homePageLayouts',
            'InboundCertificate' => 'inboundCertificates',
            'InboundNetworkConnection' => 'inboundNetworkConnections',
            'InstalledPackage' => 'installedPackages',
            'IPAddressRange' => 'IPAddressRanges',
            'KeywordList' => 'moderation',
            'Layout' => 'layouts',
            'Letterhead' => 'letterhead',
            'LightningBolt' => 'lightningBolts',
//            'LightningComponentBundle' => '', not found !!!
            'LightningExperienceTheme' => 'lightningExperienceThemes',
            'LightningMessageChannel' => 'messageChannels',
            'LightningOnboardingConfig' => 'LightningOnboardingConfigs',
            'LiveChatAgentConfig' => 'liveChatAgentConfigs',
            'LiveChatButton' => 'liveChatButtons',
            'LiveChatDeployment' => 'liveChatDeployments',
            'LiveChatSensitiveDataRule' => 'liveChatSensitiveDataRule',
            'ManagedContentType' => 'managedContentTypes',
            'ManagedTopics' => 'managedTopics',
            'MatchingRule' => 'matchingRules',
//            'Metadata' => '', not found !!!
//            'MetadataWithContent' => '', not found !!!
            'MilestoneType' => 'milestoneTypes',
            'MlDomain' => 'mlDomains',
            'MktCalcInsightObjectDef' => 'mktCalcInsightObjectDefs',
            'MktDataTranObject' => 'mktDataTranObjects',
            'MLDataDefinition' => 'mlDataDefinitions',
            'MLPredictionDefinition' => 'mlPredictions',
            'MobileApplicationDetail' => 'MobileApplicationDetails',
            'ModerationRule' => 'moderation',
            'MutingPermissionSet' => 'mutingpermissionsets',
            'MyDomainDiscoverableLogin' => 'myDomainDiscoverableLogins',
            'NamedCredential' => 'namedCredentials',
            'NavigationMenu' => 'navigationMenus',
            'Network' => 'networks',
            'NetworkBranding' => 'networkBranding',
            'NotificationTypeConfig' => 'notificationTypeConfig',
            'OauthCustomScope' => 'oauthcustomscopes',
            'ObjectSourceTargetMap' => 'objectSourceTargetMaps',
            'OcrSampleDocument' => 'ocrSampleDocuments',
            'OcrTemplate' => 'ocrTemplates',
            'OutboundNetworkConnection' => 'outboundNetworkConnections',
//            'Package' => '', not found !!!
            'PathAssistant' => 'pathAssistants',
            'PaymentGatewayProvider' => 'paymentGatewayProviders',
//            'PermissionSet' => '', not found !!!
            'PermissionSetGroup' => 'permissionsetgroups',
            'PlatformCachePartition' => 'cachePartitions',
            'PlatformEventChannel' => 'platformEventChannels',
            'PlatformEventChannelMember' => 'platformEventChannelMembers',
            'PlatformEventSubscriberConfig' => 'PlatformEventSubscriberConfigs',
            'Portal' => 'portals',
            'PostTemplate' => 'postTemplates',
            'PresenceDeclineReason' => 'presenceDeclineReasons',
            'PresenceUserConfig' => 'presenceUserConfigs',
            'Profile' => 'profiles',
//            'ProfileActionOverride' => '', not found, Profile-based action overrides are defined as part of a custom application or profile !!!
            'ProfilePasswordPolicy' => 'profilePasswordPolicies',
            'ProfileSessionSetting' => 'profileSessionSettings',
            'Prompt' => 'prompts',
            'Queue' => 'queues',
            'QueueRoutingConfig' => 'queueRoutingConfigs',
            'QuickAction' => 'quickActions',
            'RedirectWhitelistUrl' => 'redirectWhitelistUrls',
            'RecommendationStrategy' => 'recommendationStrategies',
            'RecordActionDeployment' => 'recordActionDeployments',
            'RemoteSiteSetting' => 'remoteSiteSettings',
            'Report' => 'reports',
            'ReportType' => 'reportTypes',
            'RestrictionRule' => 'restrictionRules', // Beta
            'Role' => 'roles',
//            'RoleOrTerritory' => '', not found !!!
            'SalesWorkQueueSettings' => 'salesworkqueuesettings',
            'SamlSsoConfig' => 'samlssoconfigs',
            'Scontrol' => 'scontrols',
            'ServiceAISetupDefinition' => 'serviceAISetupDescriptions',
            'ServiceChannel' => 'serviceChannels',
            'ServicePresenceStatus' => 'servicePresenceStatuses',
            'Settings' => 'settings',
//            'SharedTo' => '', not found !!!
//            'SharingBaseRule' => '', not found !!!
            'SharingRules' => 'sharingRules', // need to be careful !!!
            'SharingSet' => 'sharingSets',
            'SiteDotCom' => 'siteDotComSites',
            'Skill' => 'skills',
            'StandardValueSet' => 'standardValueSets',
            'StandardValueSetTranslation' => 'standardValueSetTranslations',
            'StaticResource' => 'staticresources',
            'SynonymDictionary' => 'synonymDictionaries',
            'Territory' => 'territories',
            'Territory2' => 'territories', //need to be careful, stored in the territories folder under the folder for the corresponding Territory2Model !!!
            'Territory2Model' => 'territory2Models',
            'Territory2Rule' => 'rules', //need to be careful, stored in the rules folder under the folder for the corresponding Territory2Model !!!
            'Territory2Type' => 'territory2Types',
            'TimeSheetTemplate' => 'timeSheetTemplates',
            'TopicsForObjects' => 'topicsForObjects',
            'TransactionSecurityPolicy' => 'transactionSecurityPolicies',
            'Translations' => 'translations',
            'UserAuthCertificate' => 'userAuthCertificates',
            'UserCriteria' => 'UserCriteria',
            'UserProvisioningConfig' => 'UserProvisioningConfigs',
            'WaveApplication' => 'wave',
            'WaveDataflow' => 'wave',
            'WaveDashboard' => 'wave',
            'WaveDataset' => 'wave',
            'WaveLens' => 'wave',
            'WaveRecipe' => 'wave',
            'WaveTemplateBundle' => 'waveTemplates',
            'WaveXmd' => 'wave',
            'WebStoreTemplate' => 'webstoretemplate',
            'Workflow' => 'workflows',
            'WorkSkillRouting' => 'workSkillRoutings'
    };</pre>
<b>Metatypes suffixes (extensions) map</b>
<pre>   public static final Map<String, String> metaTypeSuffixMap = new Map<String, String> {
            'AccountRelationshipShareRule' => 'accountRelationshipShareRule',
            'ActionLinkGroupTemplate' => 'actionLinkGroupTemplate',
            'ActionPlanTemplate' => 'apt',
            'AIApplication' => 'ai',
            'AIApplicationConfig' => 'aiapplicationconfig',
            'AnalyticSnapshot' => 'snapshot',
            'AnimationRule' => 'animationRule',
            'ArticleType' => '__kav', //need to be careful, example: newarticle__kav.description__c !!!
            'ApexClass' => 'cls',
            'ApexComponent' => 'component',
            'ApexEmailNotifications' => 'notifications', // example: apexEmailNotifications.notifications
            'ApexPage' => 'page',
            'ApexTestSuite' => 'testSuite',
            'ApexTrigger' => 'trigger',
//            'AppMenu' => '',  not found !!!
            'AppointmentAssignmentPolicy' => 'policy',
            'AppointmentSchedulingPolicy' => 'policy',
            'ApprovalProcess' => 'approvalProcess',
            'AssignmentRules' => 'assignmentRules', // For example, all Case assignment rules are stored in the Case.assignmentRules file.
            'Audience' => 'audience',
//            'AuraDefinitionBundle' => ''  can be 'app','cmp','design','evt','intf','js','svg','css','auradoc','tokens' !!!
            'AuthProvider' => 'authprovider',
            'AutoResponseRules' => 'autoResponseRules',
            'BatchCalcJobDefinition' => 'batchCalcJobDefinition',
            'BatchProcessJobDefinition' => 'batchProcessJobDefinition',
            'Bot' => 'bot',
            'BotVersion' => 'bot',
            'BrandingSet' => 'brandingSet',
            'BriefcaseDefinition' => 'briefcaseDefinition',
            'BusinessProcessGroup' => 'businessProcessGroup',
            'CallCenter' => 'callCenter',
            'CallCoachingMediaProvider' => 'callCoachingMediaProvider',
            'CampaignInfluenceModel' => 'campaignInfluenceModel',
            'CaseSubjectParticle' => 'CaseSubjectParticle',
            'CareSystemFieldMapping' => 'careSystemFieldMapping',
            'CareProviderSearchConfig' => 'careProviderSearchConfig',
            'Certificate' => 'crt',
//            'ChatterExtension' => '', not found !!!
            'CleanDataService' => 'cleanDataService',
            'CMSConnectSource' => 'cmsConnectSource',
            'Community' => 'community', // In API version 28, the API object label has changed to Zone, but the API type is still Community !!!
            'Zone' => 'community', // In API version 28, the API object label has changed to Zone, but the API type is still Community !!!
            'CommunityTemplateDefinition' => 'communityTemplateDefinition',
            'CommunityThemeDefinition' => 'communityThemeDefinition',
            'ConnectedApp' => 'connectedApp',
            'ContentAsset' => 'asset',
            'CorsWhitelistOrigin' => 'corswhitelistorigin',
            'CspTrustedSite' => 'cspTrustedSite',
            'CustomApplication' => 'app',
            'CustomApplicationComponent' => 'customApplicationComponent',
            'CustomFeedFilter' => 'feedFilter',
            'CustomHelpMenuSection' => 'customHelpMenuSection',
//            'CustomLabels' => '', not found, all custom labels store in 'labels/CustomLabels.labels' !!!
            'CustomMetadata' => '__mdt', // need to be careful !!!
            'CustomNotificationType' => 'notiftype',
            'CustomObject' => 'object',
            'CustomObjectTranslation' => 'objectTranslation', // need to be careful !!!
            'CustomPageWebLink' => 'weblink',
            'CustomPermission' => 'customPermission',
            'CustomSite' => 'site',
            'CustomTab' => 'tab',
            'CustomValue' => 'customValue',
            'Dashboard' => 'dashboard',
            'DataCategoryGroup' => 'datacategorygroup',
            'DataPackageKitObject' => 'DataPackageKitObject',
            'DataConnectorS3' => 's3DataConnector',
            'DataSource' => 'dataSource',
            'DataSourceObject' => 'dataSourceObject',
            'DataStreamDefinition' => 'dataStreamDefinition',
            'DecisionTable' => 'decisionTable',
            'DecisionTableDatasetLink' => 'decisionTableDatasetLink',
            'DelegateGroup' => 'delegateGroup',
            'DiscoveryAIModel' => 'model',
            'DiscoveryGoal' => 'goal',
//            'Document' => '', can be different suffixes
            'DuplicateRule' => 'duplicateRule',
            'EclairGeoData' => 'geodata',
            'EmailServicesFunction' => 'xml',
            'EmailTemplate' => 'email',
//            'EmbeddedServiceBranding' => '', not found !!!
//            'EmbeddedServiceConfig' => '', not found !!!
//            'EmbeddedServiceFieldService' => '', not found !!!
//            'EmbeddedServiceFlowConfig' => '', not found !!!
//            'EmbeddedServiceLiveAgent' => '', not found !!!
//            'EmbeddedServiceMenuSettings' => '', not found !!!
            'EntitlementProcess' => 'entitlementProcess', // need to be careful !!!
            'EntitlementTemplate' => 'entitlementTemplate',
            'EscalationRules' => 'escalationRules',
            'EventDelivery' => 'delivery',
            'EventSubscription' => 'subscription',
            'ExperienceBundle' => 'json', // need to be careful !!!
            'ExternalDataConnector' => 'externalDataConnector',
            'ExternalDataSource' => 'dataSource',
            'ExternalServiceRegistration' => 'dataSource',
            'FeatureParameterBoolean' => 'featureParameterBoolean',
            'FeatureParameterDate' => 'featureParameterDate',
            'FeatureParameterInteger' => 'featureParameterInteger',
            'FieldRestrictionRule' => 'rule',
            'FieldSrcTrgtRelationship' => 'fieldSrcTrgtRelationship',
            'FlexiPage' => 'flow',
            'FlowCategory' => 'flowCategory',
            'FlowDefinition' => 'flowDefinition',
            'Folder' => '-meta.xml', // need be careful !!!
            'ForecastingSourceDefinition' => 'forecastingSourceDefinition',
            'ForecastingType' => 'forecastingType',
            'ForecastingTypeSource' => 'forecastingTypeSource',
            'FunctionReference' => 'functions',
//            'GatewayProviderPaymentMethodType' => '', not found !!!
            'GlobalPicklist' => 'globalPicklist',
//            'GlobalPicklistValue' => '', not found !!!
            'GlobalValueSet' => 'globalValueSet',
            'GlobalValueSetTranslation' => 'globalValueSetTranslation', // need be careful !!!
            'Group' => 'group',
            'HomePageLayout' => 'homePageLayout',
            'InboundCertificate' => 'inboundCertificate',
            'InboundNetworkConnection' => 'inboundNetworkConnection',
            'InstalledPackage' => 'installedPackage', // need be careful !!!
            'IPAddressRange' => 'IPAddressRange',
            'KeywordList' => 'keywords',
            'Layout' => 'layout',
            'Letterhead' => 'letter',
            'LightningBolt' => 'lightningBolt',
//            'LightningComponentBundle' => '', not found !!!
            'LightningExperienceTheme' => 'lightningExperienceTheme',
            'LightningMessageChannel' => 'messageChannel',
            'LightningOnboardingConfig' => 'lightningOnboardingConfig',
            'LiveChatAgentConfig' => 'liveChatAgentConfig',
            'LiveChatButton' => 'liveChatButton',
            'LiveChatDeployment' => 'liveChatDeployment',
            'LiveChatSensitiveDataRule' => 'liveChatSensitiveDataRule',
            'ManagedContentType' => 'managedContentType',
            'ManagedTopics' => 'managedTopics',
            'MatchingRule' => 'matchingRule',
//            'Metadata' => '', not found !!!
//            'MetadataWithContent' => '', not found !!!
            'MilestoneType' => 'milestoneType',
            'MlDomain' => 'mlDomain',
            'MktCalcInsightObjectDef' => 'mktCalcInsightObjectDef',
            'MktDataTranObject' => 'mktDataTranObject',
            'MLDataDefinition' => 'mlDataDefinition',
            'MLPredictionDefinition' => 'mlPrediction',
            'MobileApplicationDetail' => 'MobileApplicationDetail',
            'ModerationRule' => 'rule', // need be careful !!!
            'MutingPermissionSet' => 'mutingpermissionset',
            'MyDomainDiscoverableLogin' => 'myDomainDiscoverableLogin',
            'NamedCredential' => 'namedCredential',
            'NavigationMenu' => 'navigationMenu',
            'Network' => 'network',
            'NetworkBranding' => 'networkBranding',
            'NotificationTypeConfig' => 'config',
            'OauthCustomScope' => 'oauthcustomscope',
            'ObjectSourceTargetMap' => 'objectSourceTargetMap',
            'OcrSampleDocument' => 'ocrSampleDocument',
            'OcrTemplate' => 'ocrTemplate',
            'OutboundNetworkConnection' => 'outboundNetworkConnection',
//            'Package' => '', not found !!!
            'PathAssistant' => 'pathAssistant',
            'PaymentGatewayProvider' => 'paymentGatewayProvider',
//            'PermissionSet' => '', not found !!!
            'PermissionSetGroup' => 'permissionsetgroup',
            'PlatformCachePartition' => 'cachePartition',
            'PlatformEventChannel' => 'platformEventChannel',
            'PlatformEventChannelMember' => 'platformEventChannelMember',
            'PlatformEventSubscriberConfig' => 'platformEventSubscriberConfig',
            'Portal' => 'portal',
            'PostTemplate' => 'postTemplate',
            'PresenceDeclineReason' => 'presenceDeclineReason',
            'PresenceUserConfig' => 'presenceUserConfig',
            'Profile' => 'profile',
//            'ProfileActionOverride' => '', not found, Profile-based action overrides are defined as part of a custom application or profile !!!
            'ProfilePasswordPolicy' => 'profilePasswordPolicy',
            'ProfileSessionSetting' => 'profileSessionSetting',
            'Prompt' => 'prompt',
            'Queue' => 'queue',
            'QueueRoutingConfig' => 'queueRoutingConfig',
            'QuickAction' => 'quickAction',
            'RedirectWhitelistUrl' => 'redirectWhitelistUrl',
            'RecommendationStrategy' => 'recommendationStrategy',
            'RecordActionDeployment' => 'deployment', // need to be careful !!!
            'RemoteSiteSetting' => 'remoteSite',
            'Report' => 'report',
            'ReportType' => 'reportType',
            'RestrictionRule' => 'rule', // Beta
            'Role' => 'role',
//            'RoleOrTerritory' => '', not found !!!
            'SalesWorkQueueSettings' => 'salesworkqueuesetting',
            'SamlSsoConfig' => 'samlssoconfig',
            'Scontrol' => 'scf',
            'ServiceAISetupDefinition' => 'serviceAISetupDescription',
            'ServiceChannel' => 'serviceChannel',
            'ServicePresenceStatus' => 'servicePresenceStatus',
            'Settings' => 'settings', // need to be careful !!!
//            'SharedTo' => '', not found !!!
//            'SharingBaseRule' => '', not found !!!
            'SharingRules' => 'sharingRules', // need to be careful !!!
            'SharingSet' => 'sharingSet',
            'SiteDotCom' => 'site', // need to be careful !!!
            'Skill' => 'skill',
            'StandardValueSet' => 'standardValueSet',
            'StandardValueSetTranslation' => 'standardValueSetTranslation', //need to be careful !!!
            'StaticResource' => 'resource',
            'SynonymDictionary' => 'synonymDictionary',
            'Territory' => 'territory',
            'Territory2' => 'territory2',
            'Territory2Model' => 'territory2Rule',
            'Territory2Type' => 'territory2Type',
            'TimeSheetTemplate' => 'timeSheetTemplate',
            'TopicsForObjects' => 'topicsForObjects',
            'TransactionSecurityPolicy' => 'transactionSecurityPolicy',
            'Translations' => 'translation', // need to be careful !!!
            'UserAuthCertificate' => 'userAuthCertificate',
            'UserCriteria' => 'userCriteria', // need to be careful !!!
            'UserProvisioningConfig' => 'userProvisioningConfig',
            'WaveApplication' => 'wapp',
            'WaveDataflow' => 'wdf',
            'WaveDashboard' => 'wdash',
            'WaveDataset' => 'wds',
            'WaveLens' => 'wlens',
            'WaveRecipe' => 'wdpr',
//            'WaveTemplateBundle' => '', not found !!!
            'WaveXmd' => 'xmd',
            'WebStoreTemplate' => 'webstoretemplate',
            'Workflow' => 'workflow',
            'WorkSkillRouting' => 'workSkillRouting'
    };</pre>
