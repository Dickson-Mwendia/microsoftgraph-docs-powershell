---
external help file: Microsoft.Graph.Beta.DeviceManagement.Administration-help.xml
Module Name: Microsoft.Graph.Beta.DeviceManagement.Administration
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.devicemanagement.administration/update-mgbetadevicemanagementvirtualendpointgalleryimage
schema: 2.0.0
---

# Update-MgBetaDeviceManagementVirtualEndpointGalleryImage

## SYNOPSIS
Update the navigation property galleryImages in deviceManagement

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgBetaDeviceManagementVirtualEndpointGalleryImage -CloudPcGalleryImageId <String>
 [-AdditionalProperties <Hashtable>] [-DisplayName <String>] [-EndDate <DateTime>] [-ExpirationDate <DateTime>]
 [-Id <String>] [-Offer <String>] [-OfferDisplayName <String>] [-Publisher <String>] [-RecommendedSku <String>]
 [-SizeInGb <Int32>] [-Sku <String>] [-SkuDisplayName <String>] [-StartDate <DateTime>] [-Status <String>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Update
```
Update-MgBetaDeviceManagementVirtualEndpointGalleryImage -CloudPcGalleryImageId <String>
 -BodyParameter <IMicrosoftGraphCloudPcGalleryImage> [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentityExpanded
```
Update-MgBetaDeviceManagementVirtualEndpointGalleryImage -InputObject <IDeviceManagementAdministrationIdentity>
 [-AdditionalProperties <Hashtable>] [-DisplayName <String>] [-EndDate <DateTime>] [-ExpirationDate <DateTime>]
 [-Id <String>] [-Offer <String>] [-OfferDisplayName <String>] [-Publisher <String>] [-RecommendedSku <String>]
 [-SizeInGb <Int32>] [-Sku <String>] [-SkuDisplayName <String>] [-StartDate <DateTime>] [-Status <String>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentity
```
Update-MgBetaDeviceManagementVirtualEndpointGalleryImage -InputObject <IDeviceManagementAdministrationIdentity>
 -BodyParameter <IMicrosoftGraphCloudPcGalleryImage> [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Update the navigation property galleryImages in deviceManagement

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

### -BodyParameter
cloudPcGalleryImage
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphCloudPcGalleryImage
Parameter Sets: Update, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -CloudPcGalleryImageId
The unique identifier of cloudPcGalleryImage

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

### -DisplayName
The official display name of the gallery image.
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

### -EndDate
The date in which this image is no longer within long-term support.
The Cloud PC continues to provide short-term support.
Read-only.

```yaml
Type: DateTime
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ExpirationDate
The date when the image is no longer available.
Read-only.

```yaml
Type: DateTime
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
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
Type: IDeviceManagementAdministrationIdentity
Parameter Sets: UpdateViaIdentityExpanded, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Offer
The offer name of the gallery image.
This value is passed to Azure to get the image resource.
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

### -OfferDisplayName
The official display offer name of the gallery image.
For example, Windows 10 Enterprise + OS Optimizations.
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

### -Publisher
The publisher name of the gallery image.
This value is passed to Azure to get the image resource.
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

### -RecommendedSku
Recommended Cloud PC SKU for this gallery image.
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

### -SizeInGb
The size of this image in gigabytes.
Read-only.

```yaml
Type: Int32
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -Sku
The SKU name of the gallery image.
This value is passed to Azure to get the image resource.
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

### -SkuDisplayName
The official display stock keeping unit (SKU) name of this gallery image.
For example, 2004.
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

### -StartDate
The date when the image becomes available.
Read-only.

```yaml
Type: DateTime
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Status
cloudPcGalleryImageStatus

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

### Microsoft.Graph.Beta.PowerShell.Models.IDeviceManagementAdministrationIdentity
### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphCloudPcGalleryImage
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphCloudPcGalleryImage
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER \<IMicrosoftGraphCloudPcGalleryImage\>: cloudPcGalleryImage
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
  \[DisplayName \<String\>\]: The official display name of the gallery image.
Read-only.
  \[EndDate \<DateTime?\>\]: The date in which this image is no longer within long-term support.
The Cloud PC continues to provide short-term support.
Read-only.
  \[ExpirationDate \<DateTime?\>\]: The date when the image is no longer available.
Read-only.
  \[Offer \<String\>\]: The offer name of the gallery image.
This value is passed to Azure to get the image resource.
Read-only.
  \[OfferDisplayName \<String\>\]: The official display offer name of the gallery image.
For example, Windows 10 Enterprise + OS Optimizations.
Read-only.
  \[Publisher \<String\>\]: The publisher name of the gallery image.
This value is passed to Azure to get the image resource.
Read-only.
  \[RecommendedSku \<String\>\]: Recommended Cloud PC SKU for this gallery image.
Read-only.
  \[SizeInGb \<Int32?\>\]: The size of this image in gigabytes.
Read-only.
  \[Sku \<String\>\]: The SKU name of the gallery image.
This value is passed to Azure to get the image resource.
Read-only.
  \[SkuDisplayName \<String\>\]: The official display stock keeping unit (SKU) name of this gallery image.
For example, 2004.
Read-only.
  \[StartDate \<DateTime?\>\]: The date when the image becomes available.
Read-only.
  \[Status \<String\>\]: cloudPcGalleryImageStatus

INPUTOBJECT \<IDeviceManagementAdministrationIdentity\>: Identity Parameter
  \[AuditEventId \<String\>\]: The unique identifier of auditEvent
  \[CartToClassAssociationId \<String\>\]: The unique identifier of cartToClassAssociation
  \[CloudPcAuditEventId \<String\>\]: The unique identifier of cloudPcAuditEvent
  \[CloudPcBulkActionId \<String\>\]: The unique identifier of cloudPcBulkAction
  \[CloudPcDeviceImageId \<String\>\]: The unique identifier of cloudPcDeviceImage
  \[CloudPcExportJobId \<String\>\]: The unique identifier of cloudPcExportJob
  \[CloudPcExternalPartnerSettingId \<String\>\]: The unique identifier of cloudPcExternalPartnerSetting
  \[CloudPcFrontLineServicePlanId \<String\>\]: The unique identifier of cloudPcFrontLineServicePlan
  \[CloudPcGalleryImageId \<String\>\]: The unique identifier of cloudPcGalleryImage
  \[CloudPcId \<String\>\]: The unique identifier of cloudPC
  \[CloudPcOnPremisesConnectionId \<String\>\]: The unique identifier of cloudPcOnPremisesConnection
  \[CloudPcProvisioningPolicyAssignmentId \<String\>\]: The unique identifier of cloudPcProvisioningPolicyAssignment
  \[CloudPcProvisioningPolicyId \<String\>\]: The unique identifier of cloudPcProvisioningPolicy
  \[CloudPcServicePlanId \<String\>\]: The unique identifier of cloudPcServicePlan
  \[CloudPcSharedUseServicePlanId \<String\>\]: The unique identifier of cloudPcSharedUseServicePlan
  \[CloudPcSnapshotId \<String\>\]: The unique identifier of cloudPcSnapshot
  \[CloudPcSupportedRegionId \<String\>\]: The unique identifier of cloudPcSupportedRegion
  \[CloudPcUserSettingAssignmentId \<String\>\]: The unique identifier of cloudPcUserSettingAssignment
  \[CloudPcUserSettingId \<String\>\]: The unique identifier of cloudPcUserSetting
  \[ComanagementEligibleDeviceId \<String\>\]: The unique identifier of comanagementEligibleDevice
  \[ComplianceManagementPartnerId \<String\>\]: The unique identifier of complianceManagementPartner
  \[DeviceAndAppManagementRoleAssignmentId \<String\>\]: The unique identifier of deviceAndAppManagementRoleAssignment
  \[DeviceManagementDomainJoinConnectorId \<String\>\]: The unique identifier of deviceManagementDomainJoinConnector
  \[DeviceManagementExchangeConnectorId \<String\>\]: The unique identifier of deviceManagementExchangeConnector
  \[DeviceManagementExchangeOnPremisesPolicyId \<String\>\]: The unique identifier of deviceManagementExchangeOnPremisesPolicy
  \[DeviceManagementPartnerId \<String\>\]: The unique identifier of deviceManagementPartner
  \[GroupPolicyCategoryId \<String\>\]: The unique identifier of groupPolicyCategory
  \[GroupPolicyCategoryId1 \<String\>\]: The unique identifier of groupPolicyCategory
  \[GroupPolicyDefinitionFileId \<String\>\]: The unique identifier of groupPolicyDefinitionFile
  \[GroupPolicyDefinitionId \<String\>\]: The unique identifier of groupPolicyDefinition
  \[GroupPolicyMigrationReportId \<String\>\]: The unique identifier of groupPolicyMigrationReport
  \[GroupPolicyObjectFileId \<String\>\]: The unique identifier of groupPolicyObjectFile
  \[GroupPolicyOperationId \<String\>\]: The unique identifier of groupPolicyOperation
  \[GroupPolicyPresentationId \<String\>\]: The unique identifier of groupPolicyPresentation
  \[GroupPolicySettingMappingId \<String\>\]: The unique identifier of groupPolicySettingMapping
  \[GroupPolicyUploadedDefinitionFileId \<String\>\]: The unique identifier of groupPolicyUploadedDefinitionFile
  \[IntuneBrandingProfileAssignmentId \<String\>\]: The unique identifier of intuneBrandingProfileAssignment
  \[IntuneBrandingProfileId \<String\>\]: The unique identifier of intuneBrandingProfile
  \[IosUpdateDeviceStatusId \<String\>\]: The unique identifier of iosUpdateDeviceStatus
  \[ManagedAllDeviceCertificateStateId \<String\>\]: The unique identifier of managedAllDeviceCertificateState
  \[MobileThreatDefenseConnectorId \<String\>\]: The unique identifier of mobileThreatDefenseConnector
  \[NdesConnectorId \<String\>\]: The unique identifier of ndesConnector
  \[RemoteAssistancePartnerId \<String\>\]: The unique identifier of remoteAssistancePartner
  \[ResourceOperationId \<String\>\]: The unique identifier of resourceOperation
  \[RestrictedAppsViolationId \<String\>\]: The unique identifier of restrictedAppsViolation
  \[RoleAssignmentId \<String\>\]: The unique identifier of roleAssignment
  \[RoleDefinitionId \<String\>\]: The unique identifier of roleDefinition
  \[RoleScopeTagAutoAssignmentId \<String\>\]: The unique identifier of roleScopeTagAutoAssignment
  \[RoleScopeTagId \<String\>\]: The unique identifier of roleScopeTag
  \[TelecomExpenseManagementPartnerId \<String\>\]: The unique identifier of telecomExpenseManagementPartner
  \[TermsAndConditionsAcceptanceStatusId \<String\>\]: The unique identifier of termsAndConditionsAcceptanceStatus
  \[TermsAndConditionsAssignmentId \<String\>\]: The unique identifier of termsAndConditionsAssignment
  \[TermsAndConditionsGroupAssignmentId \<String\>\]: The unique identifier of termsAndConditionsGroupAssignment
  \[TermsAndConditionsId \<String\>\]: The unique identifier of termsAndConditions
  \[UnsupportedGroupPolicyExtensionId \<String\>\]: The unique identifier of unsupportedGroupPolicyExtension
  \[UserId \<String\>\]: The unique identifier of user
  \[UserPfxCertificateId \<String\>\]: The unique identifier of userPFXCertificate

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.devicemanagement.administration/update-mgbetadevicemanagementvirtualendpointgalleryimage](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.devicemanagement.administration/update-mgbetadevicemanagementvirtualendpointgalleryimage)



