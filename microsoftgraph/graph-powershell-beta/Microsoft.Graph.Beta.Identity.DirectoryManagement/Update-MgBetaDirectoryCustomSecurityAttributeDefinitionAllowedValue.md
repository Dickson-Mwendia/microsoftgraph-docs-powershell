---
external help file: Microsoft.Graph.Beta.Identity.DirectoryManagement-help.xml
Module Name: Microsoft.Graph.Beta.Identity.DirectoryManagement
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.directorymanagement/update-mgbetadirectorycustomsecurityattributedefinitionallowedvalue
schema: 2.0.0
ms.prod: directory-management
---

# Update-MgBetaDirectoryCustomSecurityAttributeDefinitionAllowedValue

## SYNOPSIS
Update the properties of an allowedValue object.
This API is available in the following national cloud deployments.

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [Update-MgDirectoryCustomSecurityAttributeDefinitionAllowedValue](/powershell/module/Microsoft.Graph.Identity.DirectoryManagement/Update-MgDirectoryCustomSecurityAttributeDefinitionAllowedValue?view=graph-powershell-1.0)

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgBetaDirectoryCustomSecurityAttributeDefinitionAllowedValue -AllowedValueId <String>
 -CustomSecurityAttributeDefinitionId <String> [-AdditionalProperties <Hashtable>] [-Id <String>] [-IsActive]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Update
```
Update-MgBetaDirectoryCustomSecurityAttributeDefinitionAllowedValue -AllowedValueId <String>
 -CustomSecurityAttributeDefinitionId <String> -BodyParameter <IMicrosoftGraphAllowedValue> [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentityExpanded
```
Update-MgBetaDirectoryCustomSecurityAttributeDefinitionAllowedValue
 -InputObject <IIdentityDirectoryManagementIdentity> [-AdditionalProperties <Hashtable>] [-Id <String>]
 [-IsActive] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentity
```
Update-MgBetaDirectoryCustomSecurityAttributeDefinitionAllowedValue
 -InputObject <IIdentityDirectoryManagementIdentity> -BodyParameter <IMicrosoftGraphAllowedValue> [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Update the properties of an allowedValue object.
This API is available in the following national cloud deployments.

## EXAMPLES
### Example 1: Using the Update-MgBetaDirectoryCustomSecurityAttributeDefinitionAllowedValue Cmdlet
```powershell
Import-Module Microsoft.Graph.Beta.Identity.DirectoryManagement
$params = @{
	IsActive = "false"
}
Update-MgBetaDirectoryCustomSecurityAttributeDefinitionAllowedValue -CustomSecurityAttributeDefinitionId $customSecurityAttributeDefinitionId -AllowedValueId $allowedValueId -BodyParameter $params
```
This example shows how to use the Update-MgBetaDirectoryCustomSecurityAttributeDefinitionAllowedValue Cmdlet.
To learn about permissions for this resource, see the [permissions reference](/graph/permissions-reference).

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AllowedValueId
The unique identifier of allowedValue

```yaml
Type: String
Parameter Sets: UpdateExpanded, Update
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
allowedValue
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphAllowedValue
Parameter Sets: Update, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -CustomSecurityAttributeDefinitionId
The unique identifier of customSecurityAttributeDefinition

```yaml
Type: String
Parameter Sets: UpdateExpanded, Update
Aliases:

Required: True
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
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
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
Type: IIdentityDirectoryManagementIdentity
Parameter Sets: UpdateViaIdentityExpanded, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -IsActive
Indicates whether the predefined value is active or deactivated.
If set to false, this predefined value can't be assigned to any more supported directory objects.

```yaml
Type: SwitchParameter
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: False
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

### Microsoft.Graph.Beta.PowerShell.Models.IIdentityDirectoryManagementIdentity
### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphAllowedValue
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphAllowedValue
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER \<IMicrosoftGraphAllowedValue\>: allowedValue
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
  \[IsActive \<Boolean?\>\]: Indicates whether the predefined value is active or deactivated.
If set to false, this predefined value can't be assigned to any more supported directory objects.

INPUTOBJECT \<IIdentityDirectoryManagementIdentity\>: Identity Parameter
  \[AdministrativeUnitId \<String\>\]: The unique identifier of administrativeUnit
  \[AllowedValueId \<String\>\]: The unique identifier of allowedValue
  \[AttributeSetId \<String\>\]: The unique identifier of attributeSet
  \[CertificateAuthorityAsEntityId \<String\>\]: The unique identifier of certificateAuthorityAsEntity
  \[CertificateBasedApplicationConfigurationId \<String\>\]: The unique identifier of certificateBasedApplicationConfiguration
  \[CommandId \<String\>\]: The unique identifier of command
  \[CompanySubscriptionId \<String\>\]: The unique identifier of companySubscription
  \[ContractId \<String\>\]: The unique identifier of contract
  \[CustomSecurityAttributeDefinitionId \<String\>\]: The unique identifier of customSecurityAttributeDefinition
  \[DeviceId \<String\>\]: The unique identifier of device
  \[DeviceLocalCredentialInfoId \<String\>\]: The unique identifier of deviceLocalCredentialInfo
  \[DirectoryObjectId \<String\>\]: The unique identifier of directoryObject
  \[DirectoryRoleId \<String\>\]: The unique identifier of directoryRole
  \[DirectoryRoleTemplateId \<String\>\]: The unique identifier of directoryRoleTemplate
  \[DirectorySettingId \<String\>\]: The unique identifier of directorySetting
  \[DirectorySettingTemplateId \<String\>\]: The unique identifier of directorySettingTemplate
  \[DomainDnsRecordId \<String\>\]: The unique identifier of domainDnsRecord
  \[DomainId \<String\>\]: The unique identifier of domain
  \[ExtensionId \<String\>\]: The unique identifier of extension
  \[FeatureRolloutPolicyId \<String\>\]: The unique identifier of featureRolloutPolicy
  \[IdentityProviderBaseId \<String\>\]: The unique identifier of identityProviderBase
  \[ImpactedResourceId \<String\>\]: The unique identifier of impactedResource
  \[InboundSharedUserProfileUserId \<String\>\]: The unique identifier of inboundSharedUserProfile
  \[InternalDomainFederationId \<String\>\]: The unique identifier of internalDomainFederation
  \[ManagedTenantAlertId \<String\>\]: The unique identifier of managedTenantAlert
  \[ManagementActionId \<String\>\]: The unique identifier of managementAction
  \[OnPremisesDirectorySynchronizationId \<String\>\]: The unique identifier of onPremisesDirectorySynchronization
  \[OrgContactId \<String\>\]: The unique identifier of orgContact
  \[OrganizationId \<String\>\]: The unique identifier of organization
  \[OrganizationalBrandingLocalizationId \<String\>\]: The unique identifier of organizationalBrandingLocalization
  \[OutboundSharedUserProfileUserId \<String\>\]: The unique identifier of outboundSharedUserProfile
  \[ProfileCardPropertyId \<String\>\]: The unique identifier of profileCardProperty
  \[RecommendationId \<String\>\]: The unique identifier of recommendation
  \[RoleTemplateId \<String\>\]: Alternate key of directoryRole
  \[ScopedRoleMembershipId \<String\>\]: The unique identifier of scopedRoleMembership
  \[SharedEmailDomainId \<String\>\]: The unique identifier of sharedEmailDomain
  \[SharedEmailDomainInvitationId \<String\>\]: The unique identifier of sharedEmailDomainInvitation
  \[SubscribedSkuId \<String\>\]: The unique identifier of subscribedSku
  \[TenantId \<String\>\]: The unique identifier of tenant
  \[TenantReferenceTenantId \<String\>\]: The unique identifier of tenantReference
  \[TenantTagId \<String\>\]: The unique identifier of tenantTag
  \[UsageRightId \<String\>\]: The unique identifier of usageRight
  \[UserId \<String\>\]: The unique identifier of user

## RELATED LINKS
[Update-MgDirectoryCustomSecurityAttributeDefinitionAllowedValue](/powershell/module/Microsoft.Graph.Identity.DirectoryManagement/Update-MgDirectoryCustomSecurityAttributeDefinitionAllowedValue?view=graph-powershell-1.0)

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.directorymanagement/update-mgbetadirectorycustomsecurityattributedefinitionallowedvalue](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.directorymanagement/update-mgbetadirectorycustomsecurityattributedefinitionallowedvalue)


