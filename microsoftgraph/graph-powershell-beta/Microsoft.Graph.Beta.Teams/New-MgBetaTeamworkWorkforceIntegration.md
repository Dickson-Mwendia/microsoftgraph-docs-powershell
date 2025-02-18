---
external help file: Microsoft.Graph.Beta.Teams-help.xml
Module Name: Microsoft.Graph.Beta.Teams
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.teams/new-mgbetateamworkworkforceintegration
schema: 2.0.0
---

# New-MgBetaTeamworkWorkforceIntegration

## SYNOPSIS
Create a new workforceIntegration object.
This API is available in the following national cloud deployments.

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [New-MgTeamworkWorkforceIntegration](/powershell/module/Microsoft.Graph.Teams/New-MgTeamworkWorkforceIntegration?view=graph-powershell-1.0)

## SYNTAX

### CreateExpanded (Default)
```
New-MgBetaTeamworkWorkforceIntegration [-AdditionalProperties <Hashtable>] [-ApiVersion <Int32>]
 [-CreatedBy <IMicrosoftGraphIdentitySet>] [-DisplayName <String>]
 [-EligibilityFilteringEnabledEntities <String>] [-Encryption <IMicrosoftGraphWorkforceIntegrationEncryption>]
 [-Id <String>] [-IsActive] [-LastModifiedBy <IMicrosoftGraphIdentitySet>] [-SupportedEntities <String>]
 [-Supports <String>] [-Url <String>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgBetaTeamworkWorkforceIntegration -BodyParameter <IMicrosoftGraphWorkforceIntegration> [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create a new workforceIntegration object.
This API is available in the following national cloud deployments.

## EXAMPLES
### Example 1: Code snippet

```powershell

Import-Module Microsoft.Graph.Beta.Teams

$params = @{
	displayName = "displayName-value"
	apiVersion = 99
	encryption = @{
		protocol = "protocol-value"
		secret = "secret-value"
	}
	isActive = $true
	url = "url-value"
	supports = "supports-value"
}

New-MgBetaTeamworkWorkforceIntegration -BodyParameter $params

```
This example shows how to use the New-MgBetaTeamworkWorkforceIntegration Cmdlet.


## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ApiVersion
API version for the callback URL.
Start with 1.

```yaml
Type: Int32
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
workforceIntegration
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphWorkforceIntegration
Parameter Sets: Create
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -CreatedBy
identitySet
To construct, see NOTES section for CREATEDBY properties and create a hash table.

```yaml
Type: IMicrosoftGraphIdentitySet
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DisplayName
Name of the workforce integration.

```yaml
Type: String
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -EligibilityFilteringEnabledEntities
eligibilityFilteringEnabledEntities

```yaml
Type: String
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Encryption
workforceIntegrationEncryption
To construct, see NOTES section for ENCRYPTION properties and create a hash table.

```yaml
Type: IMicrosoftGraphWorkforceIntegrationEncryption
Parameter Sets: CreateExpanded
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
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -IsActive
Indicates whether this workforce integration is currently active and available.

```yaml
Type: SwitchParameter
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -LastModifiedBy
identitySet
To construct, see NOTES section for LASTMODIFIEDBY properties and create a hash table.

```yaml
Type: IMicrosoftGraphIdentitySet
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SupportedEntities
workforceIntegrationSupportedEntities

```yaml
Type: String
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Supports
workforceIntegrationSupportedEntities

```yaml
Type: String
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Url
Workforce Integration URL for callbacks from the Shifts service.

```yaml
Type: String
Parameter Sets: CreateExpanded
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

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphWorkforceIntegration
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphWorkforceIntegration
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER \<IMicrosoftGraphWorkforceIntegration\>: workforceIntegration
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[CreatedBy \<IMicrosoftGraphIdentitySet\>\]: identitySet
    \[(Any) \<Object\>\]: This indicates any property can be added to this object.
    \[Application \<IMicrosoftGraphIdentity\>\]: identity
      \[(Any) \<Object\>\]: This indicates any property can be added to this object.
      \[DisplayName \<String\>\]: The display name of the identity.
This might not always be available or up to date.
For example, if a user changes their display name, the API might show the new value in a future response, but the items associated with the user won't show up as having changed when using delta.
      \[Id \<String\>\]: Unique identifier for the identity.
    \[Device \<IMicrosoftGraphIdentity\>\]: identity
    \[User \<IMicrosoftGraphIdentity\>\]: identity
  \[LastModifiedBy \<IMicrosoftGraphIdentitySet\>\]: identitySet
  \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
  \[ApiVersion \<Int32?\>\]: API version for the callback URL.
Start with 1.
  \[DisplayName \<String\>\]: Name of the workforce integration.
  \[EligibilityFilteringEnabledEntities \<String\>\]: eligibilityFilteringEnabledEntities
  \[Encryption \<IMicrosoftGraphWorkforceIntegrationEncryption\>\]: workforceIntegrationEncryption
    \[(Any) \<Object\>\]: This indicates any property can be added to this object.
    \[Protocol \<String\>\]: workforceIntegrationEncryptionProtocol
    \[Secret \<String\>\]: Encryption shared secret.
  \[IsActive \<Boolean?\>\]: Indicates whether this workforce integration is currently active and available.
  \[SupportedEntities \<String\>\]: workforceIntegrationSupportedEntities
  \[Supports \<String\>\]: workforceIntegrationSupportedEntities
  \[Url \<String\>\]: Workforce Integration URL for callbacks from the Shifts service.

CREATEDBY \<IMicrosoftGraphIdentitySet\>: identitySet
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[Application \<IMicrosoftGraphIdentity\>\]: identity
    \[(Any) \<Object\>\]: This indicates any property can be added to this object.
    \[DisplayName \<String\>\]: The display name of the identity.
This might not always be available or up to date.
For example, if a user changes their display name, the API might show the new value in a future response, but the items associated with the user won't show up as having changed when using delta.
    \[Id \<String\>\]: Unique identifier for the identity.
  \[Device \<IMicrosoftGraphIdentity\>\]: identity
  \[User \<IMicrosoftGraphIdentity\>\]: identity

ENCRYPTION \<IMicrosoftGraphWorkforceIntegrationEncryption\>: workforceIntegrationEncryption
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[Protocol \<String\>\]: workforceIntegrationEncryptionProtocol
  \[Secret \<String\>\]: Encryption shared secret.

LASTMODIFIEDBY \<IMicrosoftGraphIdentitySet\>: identitySet
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[Application \<IMicrosoftGraphIdentity\>\]: identity
    \[(Any) \<Object\>\]: This indicates any property can be added to this object.
    \[DisplayName \<String\>\]: The display name of the identity.
This might not always be available or up to date.
For example, if a user changes their display name, the API might show the new value in a future response, but the items associated with the user won't show up as having changed when using delta.
    \[Id \<String\>\]: Unique identifier for the identity.
  \[Device \<IMicrosoftGraphIdentity\>\]: identity
  \[User \<IMicrosoftGraphIdentity\>\]: identity

## RELATED LINKS
[New-MgTeamworkWorkforceIntegration](/powershell/module/Microsoft.Graph.Teams/New-MgTeamworkWorkforceIntegration?view=graph-powershell-1.0)

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.teams/new-mgbetateamworkworkforceintegration](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.teams/new-mgbetateamworkworkforceintegration)


