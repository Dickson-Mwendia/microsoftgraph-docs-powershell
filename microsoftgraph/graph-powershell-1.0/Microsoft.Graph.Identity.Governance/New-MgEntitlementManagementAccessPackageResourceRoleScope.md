---
external help file: Microsoft.Graph.Identity.Governance-help.xml
Module Name: Microsoft.Graph.Identity.Governance
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.identity.governance/new-mgentitlementmanagementaccesspackageresourcerolescope
schema: 2.0.0
ms.prod: governance
---

# New-MgEntitlementManagementAccessPackageResourceRoleScope

## SYNOPSIS
Create a new accessPackageResourceRoleScope for adding a resource role to an access package.
The access package resource, for a group, an app, or a SharePoint Online site, must already exist in the access package catalog, and the originId for the resource role retrieved from the list of the resource roles.
Once you add the resource role scope to the access package, the user will receive this resource role through any current and future access package assignments.
This API is available in the following national cloud deployments.

> [!NOTE]
> To view the beta release of this cmdlet, view [New-MgBetaEntitlementManagementAccessPackageResourceRoleScope](/powershell/module/Microsoft.Graph.Beta.Identity.Governance/New-MgBetaEntitlementManagementAccessPackageResourceRoleScope?view=graph-powershell-beta)

## SYNTAX

### CreateExpanded (Default)
```
New-MgEntitlementManagementAccessPackageResourceRoleScope -AccessPackageId <String>
 [-AdditionalProperties <Hashtable>] [-CreatedDateTime <DateTime>] [-Id <String>]
 [-Role <IMicrosoftGraphAccessPackageResourceRole>] [-Scope <IMicrosoftGraphAccessPackageResourceScope>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgEntitlementManagementAccessPackageResourceRoleScope -AccessPackageId <String>
 -BodyParameter <IMicrosoftGraphAccessPackageResourceRoleScope> [-WhatIf] [-Confirm] [<CommonParameters>]
```

### CreateViaIdentityExpanded
```
New-MgEntitlementManagementAccessPackageResourceRoleScope -InputObject <IIdentityGovernanceIdentity>
 [-AdditionalProperties <Hashtable>] [-CreatedDateTime <DateTime>] [-Id <String>]
 [-Role <IMicrosoftGraphAccessPackageResourceRole>] [-Scope <IMicrosoftGraphAccessPackageResourceScope>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### CreateViaIdentity
```
New-MgEntitlementManagementAccessPackageResourceRoleScope -InputObject <IIdentityGovernanceIdentity>
 -BodyParameter <IMicrosoftGraphAccessPackageResourceRoleScope> [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create a new accessPackageResourceRoleScope for adding a resource role to an access package.
The access package resource, for a group, an app, or a SharePoint Online site, must already exist in the access package catalog, and the originId for the resource role retrieved from the list of the resource roles.
Once you add the resource role scope to the access package, the user will receive this resource role through any current and future access package assignments.
This API is available in the following national cloud deployments.

## PARAMETERS

### -AccessPackageId
The unique identifier of accessPackage

```yaml
Type: String
Parameter Sets: CreateExpanded, Create
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
accessPackageResourceRoleScope
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphAccessPackageResourceRoleScope
Parameter Sets: Create, CreateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -CreatedDateTime
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z

```yaml
Type: DateTime
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Id
The unique identifier for an entity.
Read-only.

```yaml
Type: String
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InputObject
Identity Parameter
To construct, see NOTES section for INPUTOBJECT properties and create a hash table.

```yaml
Type: IIdentityGovernanceIdentity
Parameter Sets: CreateViaIdentityExpanded, CreateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Role
accessPackageResourceRole
To construct, see NOTES section for ROLE properties and create a hash table.

```yaml
Type: IMicrosoftGraphAccessPackageResourceRole
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Scope
accessPackageResourceScope
To construct, see NOTES section for SCOPE properties and create a hash table.

```yaml
Type: IMicrosoftGraphAccessPackageResourceScope
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Confirm
Prompts you for confirmation before running the cmdlet.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
Shows what would happen if the cmdlet runs.
The cmdlet is not run.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.Graph.PowerShell.Models.IIdentityGovernanceIdentity
### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphAccessPackageResourceRoleScope
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphAccessPackageResourceRoleScope
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER \<IMicrosoftGraphAccessPackageResourceRoleScope\>: accessPackageResourceRoleScope
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
  \[CreatedDateTime \<DateTime?\>\]: The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
  \[Role \<IMicrosoftGraphAccessPackageResourceRole\>\]: accessPackageResourceRole
    \[(Any) \<Object\>\]: This indicates any property can be added to this object.
    \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
    \[Description \<String\>\]: A description for the resource role.
    \[DisplayName \<String\>\]: The display name of the resource role such as the role defined by the application.
    \[OriginId \<String\>\]: The unique identifier of the resource role in the origin system.
For a SharePoint Online site, the originId will be the sequence number of the role in the site.
    \[OriginSystem \<String\>\]: The type of the resource in the origin system, such as SharePointOnline, AadApplication or AadGroup.
    \[Resource \<IMicrosoftGraphAccessPackageResource\>\]: accessPackageResource
      \[(Any) \<Object\>\]: This indicates any property can be added to this object.
      \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
      \[CreatedDateTime \<DateTime?\>\]: The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Read-only.
      \[Description \<String\>\]: A description for the resource.
      \[DisplayName \<String\>\]: The display name of the resource, such as the application name, group name or site name.
      \[Environment \<IMicrosoftGraphAccessPackageResourceEnvironment\>\]: accessPackageResourceEnvironment
        \[(Any) \<Object\>\]: This indicates any property can be added to this object.
        \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
        \[CreatedDateTime \<DateTime?\>\]: The date and time that this object was created.
The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
        \[Description \<String\>\]: The description of this object.
        \[DisplayName \<String\>\]: The display name of this object.
        \[IsDefaultEnvironment \<Boolean?\>\]: Determines whether this is default environment or not.
It is set to true for all static origin systems, such as Microsoft Entra groups and Microsoft Entra Applications.
        \[ModifiedDateTime \<DateTime?\>\]: The date and time that this object was last modified.
The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
        \[OriginId \<String\>\]: The unique identifier of this environment in the origin system.
        \[OriginSystem \<String\>\]: The type of the resource in the origin system, that is, SharePointOnline.
Requires $filter (eq).
        \[Resources \<IMicrosoftGraphAccessPackageResource\[\]\>\]: Read-only.
Required.
      \[ModifiedDateTime \<DateTime?\>\]: The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Read-only.
      \[OriginId \<String\>\]: The unique identifier of the resource in the origin system.
In the case of a Microsoft Entra group, this is the identifier of the group.
      \[OriginSystem \<String\>\]: The type of the resource in the origin system, such as SharePointOnline, AadApplication or AadGroup.
      \[Roles \<IMicrosoftGraphAccessPackageResourceRole\[\]\>\]: Read-only.
Nullable.
Supports $expand.
      \[Scopes \<IMicrosoftGraphAccessPackageResourceScope\[\]\>\]: Read-only.
Nullable.
Supports $expand.
        \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
        \[Description \<String\>\]: The description of the scope.
        \[DisplayName \<String\>\]: The display name of the scope.
        \[IsRootScope \<Boolean?\>\]: True if the scopes are arranged in a hierarchy and this is the top or root scope of the resource.
        \[OriginId \<String\>\]: The unique identifier for the scope in the resource as defined in the origin system.
        \[OriginSystem \<String\>\]: The origin system for the scope.
        \[Resource \<IMicrosoftGraphAccessPackageResource\>\]: accessPackageResource
  \[Scope \<IMicrosoftGraphAccessPackageResourceScope\>\]: accessPackageResourceScope

INPUTOBJECT \<IIdentityGovernanceIdentity\>: Identity Parameter
  \[AccessPackageAssignmentId \<String\>\]: The unique identifier of accessPackageAssignment
  \[AccessPackageAssignmentPolicyId \<String\>\]: The unique identifier of accessPackageAssignmentPolicy
  \[AccessPackageAssignmentRequestId \<String\>\]: The unique identifier of accessPackageAssignmentRequest
  \[AccessPackageCatalogId \<String\>\]: The unique identifier of accessPackageCatalog
  \[AccessPackageId \<String\>\]: The unique identifier of accessPackage
  \[AccessPackageId1 \<String\>\]: The unique identifier of accessPackage
  \[AccessPackageQuestionId \<String\>\]: The unique identifier of accessPackageQuestion
  \[AccessPackageResourceEnvironmentId \<String\>\]: The unique identifier of accessPackageResourceEnvironment
  \[AccessPackageResourceId \<String\>\]: The unique identifier of accessPackageResource
  \[AccessPackageResourceRequestId \<String\>\]: The unique identifier of accessPackageResourceRequest
  \[AccessPackageResourceRoleId \<String\>\]: The unique identifier of accessPackageResourceRole
  \[AccessPackageResourceRoleId1 \<String\>\]: The unique identifier of accessPackageResourceRole
  \[AccessPackageResourceRoleScopeId \<String\>\]: The unique identifier of accessPackageResourceRoleScope
  \[AccessPackageResourceScopeId \<String\>\]: The unique identifier of accessPackageResourceScope
  \[AccessPackageResourceScopeId1 \<String\>\]: The unique identifier of accessPackageResourceScope
  \[AccessReviewHistoryDefinitionId \<String\>\]: The unique identifier of accessReviewHistoryDefinition
  \[AccessReviewHistoryInstanceId \<String\>\]: The unique identifier of accessReviewHistoryInstance
  \[AccessReviewInstanceDecisionItemId \<String\>\]: The unique identifier of accessReviewInstanceDecisionItem
  \[AccessReviewInstanceId \<String\>\]: The unique identifier of accessReviewInstance
  \[AccessReviewReviewerId \<String\>\]: The unique identifier of accessReviewReviewer
  \[AccessReviewScheduleDefinitionId \<String\>\]: The unique identifier of accessReviewScheduleDefinition
  \[AccessReviewStageId \<String\>\]: The unique identifier of accessReviewStage
  \[AgreementAcceptanceId \<String\>\]: The unique identifier of agreementAcceptance
  \[AgreementFileLocalizationId \<String\>\]: The unique identifier of agreementFileLocalization
  \[AgreementFileVersionId \<String\>\]: The unique identifier of agreementFileVersion
  \[AgreementId \<String\>\]: The unique identifier of agreement
  \[AppConsentRequestId \<String\>\]: The unique identifier of appConsentRequest
  \[ApprovalId \<String\>\]: The unique identifier of approval
  \[ApprovalStageId \<String\>\]: The unique identifier of approvalStage
  \[ConnectedOrganizationId \<String\>\]: The unique identifier of connectedOrganization
  \[CustomCalloutExtensionId \<String\>\]: The unique identifier of customCalloutExtension
  \[CustomExtensionStageSettingId \<String\>\]: The unique identifier of customExtensionStageSetting
  \[CustomTaskExtensionId \<String\>\]: The unique identifier of customTaskExtension
  \[DirectoryObjectId \<String\>\]: The unique identifier of directoryObject
  \[EndDateTime \<DateTime?\>\]: Usage: endDateTime={endDateTime}
  \[GovernanceInsightId \<String\>\]: The unique identifier of governanceInsight
  \[GroupId \<String\>\]: The unique identifier of group
  \[IncompatibleAccessPackageId \<String\>\]: Usage: incompatibleAccessPackageId='{incompatibleAccessPackageId}'
  \[On \<String\>\]: Usage: on='{on}'
  \[PrivilegedAccessGroupAssignmentScheduleId \<String\>\]: The unique identifier of privilegedAccessGroupAssignmentSchedule
  \[PrivilegedAccessGroupAssignmentScheduleInstanceId \<String\>\]: The unique identifier of privilegedAccessGroupAssignmentScheduleInstance
  \[PrivilegedAccessGroupAssignmentScheduleRequestId \<String\>\]: The unique identifier of privilegedAccessGroupAssignmentScheduleRequest
  \[PrivilegedAccessGroupEligibilityScheduleId \<String\>\]: The unique identifier of privilegedAccessGroupEligibilitySchedule
  \[PrivilegedAccessGroupEligibilityScheduleInstanceId \<String\>\]: The unique identifier of privilegedAccessGroupEligibilityScheduleInstance
  \[PrivilegedAccessGroupEligibilityScheduleRequestId \<String\>\]: The unique identifier of privilegedAccessGroupEligibilityScheduleRequest
  \[RunId \<String\>\]: The unique identifier of run
  \[StartDateTime \<DateTime?\>\]: Usage: startDateTime={startDateTime}
  \[TaskDefinitionId \<String\>\]: The unique identifier of taskDefinition
  \[TaskId \<String\>\]: The unique identifier of task
  \[TaskProcessingResultId \<String\>\]: The unique identifier of taskProcessingResult
  \[TaskReportId \<String\>\]: The unique identifier of taskReport
  \[UnifiedRbacResourceActionId \<String\>\]: The unique identifier of unifiedRbacResourceAction
  \[UnifiedRbacResourceNamespaceId \<String\>\]: The unique identifier of unifiedRbacResourceNamespace
  \[UnifiedRoleAssignmentId \<String\>\]: The unique identifier of unifiedRoleAssignment
  \[UnifiedRoleAssignmentScheduleId \<String\>\]: The unique identifier of unifiedRoleAssignmentSchedule
  \[UnifiedRoleAssignmentScheduleInstanceId \<String\>\]: The unique identifier of unifiedRoleAssignmentScheduleInstance
  \[UnifiedRoleAssignmentScheduleRequestId \<String\>\]: The unique identifier of unifiedRoleAssignmentScheduleRequest
  \[UnifiedRoleDefinitionId \<String\>\]: The unique identifier of unifiedRoleDefinition
  \[UnifiedRoleDefinitionId1 \<String\>\]: The unique identifier of unifiedRoleDefinition
  \[UnifiedRoleEligibilityScheduleId \<String\>\]: The unique identifier of unifiedRoleEligibilitySchedule
  \[UnifiedRoleEligibilityScheduleInstanceId \<String\>\]: The unique identifier of unifiedRoleEligibilityScheduleInstance
  \[UnifiedRoleEligibilityScheduleRequestId \<String\>\]: The unique identifier of unifiedRoleEligibilityScheduleRequest
  \[UserConsentRequestId \<String\>\]: The unique identifier of userConsentRequest
  \[UserId \<String\>\]: The unique identifier of user
  \[UserProcessingResultId \<String\>\]: The unique identifier of userProcessingResult
  \[WorkflowId \<String\>\]: The unique identifier of workflow
  \[WorkflowTemplateId \<String\>\]: The unique identifier of workflowTemplate
  \[WorkflowVersionNumber \<Int32?\>\]: The unique identifier of workflowVersion

ROLE \<IMicrosoftGraphAccessPackageResourceRole\>: accessPackageResourceRole
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
  \[Description \<String\>\]: A description for the resource role.
  \[DisplayName \<String\>\]: The display name of the resource role such as the role defined by the application.
  \[OriginId \<String\>\]: The unique identifier of the resource role in the origin system.
For a SharePoint Online site, the originId will be the sequence number of the role in the site.
  \[OriginSystem \<String\>\]: The type of the resource in the origin system, such as SharePointOnline, AadApplication or AadGroup.
  \[Resource \<IMicrosoftGraphAccessPackageResource\>\]: accessPackageResource
    \[(Any) \<Object\>\]: This indicates any property can be added to this object.
    \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
    \[CreatedDateTime \<DateTime?\>\]: The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Read-only.
    \[Description \<String\>\]: A description for the resource.
    \[DisplayName \<String\>\]: The display name of the resource, such as the application name, group name or site name.
    \[Environment \<IMicrosoftGraphAccessPackageResourceEnvironment\>\]: accessPackageResourceEnvironment
      \[(Any) \<Object\>\]: This indicates any property can be added to this object.
      \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
      \[CreatedDateTime \<DateTime?\>\]: The date and time that this object was created.
The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
      \[Description \<String\>\]: The description of this object.
      \[DisplayName \<String\>\]: The display name of this object.
      \[IsDefaultEnvironment \<Boolean?\>\]: Determines whether this is default environment or not.
It is set to true for all static origin systems, such as Microsoft Entra groups and Microsoft Entra Applications.
      \[ModifiedDateTime \<DateTime?\>\]: The date and time that this object was last modified.
The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
      \[OriginId \<String\>\]: The unique identifier of this environment in the origin system.
      \[OriginSystem \<String\>\]: The type of the resource in the origin system, that is, SharePointOnline.
Requires $filter (eq).
      \[Resources \<IMicrosoftGraphAccessPackageResource\[\]\>\]: Read-only.
Required.
    \[ModifiedDateTime \<DateTime?\>\]: The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Read-only.
    \[OriginId \<String\>\]: The unique identifier of the resource in the origin system.
In the case of a Microsoft Entra group, this is the identifier of the group.
    \[OriginSystem \<String\>\]: The type of the resource in the origin system, such as SharePointOnline, AadApplication or AadGroup.
    \[Roles \<IMicrosoftGraphAccessPackageResourceRole\[\]\>\]: Read-only.
Nullable.
Supports $expand.
    \[Scopes \<IMicrosoftGraphAccessPackageResourceScope\[\]\>\]: Read-only.
Nullable.
Supports $expand.
      \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
      \[Description \<String\>\]: The description of the scope.
      \[DisplayName \<String\>\]: The display name of the scope.
      \[IsRootScope \<Boolean?\>\]: True if the scopes are arranged in a hierarchy and this is the top or root scope of the resource.
      \[OriginId \<String\>\]: The unique identifier for the scope in the resource as defined in the origin system.
      \[OriginSystem \<String\>\]: The origin system for the scope.
      \[Resource \<IMicrosoftGraphAccessPackageResource\>\]: accessPackageResource

SCOPE \<IMicrosoftGraphAccessPackageResourceScope\>: accessPackageResourceScope
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
  \[Description \<String\>\]: The description of the scope.
  \[DisplayName \<String\>\]: The display name of the scope.
  \[IsRootScope \<Boolean?\>\]: True if the scopes are arranged in a hierarchy and this is the top or root scope of the resource.
  \[OriginId \<String\>\]: The unique identifier for the scope in the resource as defined in the origin system.
  \[OriginSystem \<String\>\]: The origin system for the scope.
  \[Resource \<IMicrosoftGraphAccessPackageResource\>\]: accessPackageResource
    \[(Any) \<Object\>\]: This indicates any property can be added to this object.
    \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
    \[CreatedDateTime \<DateTime?\>\]: The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Read-only.
    \[Description \<String\>\]: A description for the resource.
    \[DisplayName \<String\>\]: The display name of the resource, such as the application name, group name or site name.
    \[Environment \<IMicrosoftGraphAccessPackageResourceEnvironment\>\]: accessPackageResourceEnvironment
      \[(Any) \<Object\>\]: This indicates any property can be added to this object.
      \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
      \[CreatedDateTime \<DateTime?\>\]: The date and time that this object was created.
The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
      \[Description \<String\>\]: The description of this object.
      \[DisplayName \<String\>\]: The display name of this object.
      \[IsDefaultEnvironment \<Boolean?\>\]: Determines whether this is default environment or not.
It is set to true for all static origin systems, such as Microsoft Entra groups and Microsoft Entra Applications.
      \[ModifiedDateTime \<DateTime?\>\]: The date and time that this object was last modified.
The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
      \[OriginId \<String\>\]: The unique identifier of this environment in the origin system.
      \[OriginSystem \<String\>\]: The type of the resource in the origin system, that is, SharePointOnline.
Requires $filter (eq).
      \[Resources \<IMicrosoftGraphAccessPackageResource\[\]\>\]: Read-only.
Required.
    \[ModifiedDateTime \<DateTime?\>\]: The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Read-only.
    \[OriginId \<String\>\]: The unique identifier of the resource in the origin system.
In the case of a Microsoft Entra group, this is the identifier of the group.
    \[OriginSystem \<String\>\]: The type of the resource in the origin system, such as SharePointOnline, AadApplication or AadGroup.
    \[Roles \<IMicrosoftGraphAccessPackageResourceRole\[\]\>\]: Read-only.
Nullable.
Supports $expand.
      \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
      \[Description \<String\>\]: A description for the resource role.
      \[DisplayName \<String\>\]: The display name of the resource role such as the role defined by the application.
      \[OriginId \<String\>\]: The unique identifier of the resource role in the origin system.
For a SharePoint Online site, the originId will be the sequence number of the role in the site.
      \[OriginSystem \<String\>\]: The type of the resource in the origin system, such as SharePointOnline, AadApplication or AadGroup.
      \[Resource \<IMicrosoftGraphAccessPackageResource\>\]: accessPackageResource
    \[Scopes \<IMicrosoftGraphAccessPackageResourceScope\[\]\>\]: Read-only.
Nullable.
Supports $expand.

## RELATED LINKS
[New-MgBetaEntitlementManagementAccessPackageResourceRoleScope](/powershell/module/Microsoft.Graph.Beta.Identity.Governance/New-MgBetaEntitlementManagementAccessPackageResourceRoleScope?view=graph-powershell-beta)

[https://learn.microsoft.com/powershell/module/microsoft.graph.identity.governance/new-mgentitlementmanagementaccesspackageresourcerolescope](https://learn.microsoft.com/powershell/module/microsoft.graph.identity.governance/new-mgentitlementmanagementaccesspackageresourcerolescope)



