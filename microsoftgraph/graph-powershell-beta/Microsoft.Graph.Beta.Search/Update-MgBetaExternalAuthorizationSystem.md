---
external help file: Microsoft.Graph.Beta.Search-help.xml
Module Name: Microsoft.Graph.Beta.Search
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.search/update-mgbetaexternalauthorizationsystem
schema: 2.0.0
---

# Update-MgBetaExternalAuthorizationSystem

## SYNOPSIS
Update the navigation property authorizationSystems in external

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgBetaExternalAuthorizationSystem -AuthorizationSystemId <String> [-AdditionalProperties <Hashtable>]
 [-AuthorizationSystemId1 <String>] [-AuthorizationSystemName <String>] [-AuthorizationSystemType <String>]
 [-DataCollectionInfo <IMicrosoftGraphDataCollectionInfo>] [-Id <String>] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### UpdateViaIdentityExpanded
```
Update-MgBetaExternalAuthorizationSystem [-AuthorizationSystemId <String>] -InputObject <ISearchIdentity>
 [-AdditionalProperties <Hashtable>] [-AuthorizationSystemName <String>] [-AuthorizationSystemType <String>]
 [-DataCollectionInfo <IMicrosoftGraphDataCollectionInfo>] [-Id <String>] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### Update
```
Update-MgBetaExternalAuthorizationSystem -AuthorizationSystemId <String>
 -BodyParameter <IMicrosoftGraphAuthorizationSystem> [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentity
```
Update-MgBetaExternalAuthorizationSystem -InputObject <ISearchIdentity>
 -BodyParameter <IMicrosoftGraphAuthorizationSystem> [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Update the navigation property authorizationSystems in external

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

### -AuthorizationSystemId
The unique identifier of authorizationSystem

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

```yaml
Type: String
Parameter Sets: UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AuthorizationSystemId1
.

```yaml
Type: String
Parameter Sets: UpdateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AuthorizationSystemName
.

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

### -AuthorizationSystemType
.

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

### -BodyParameter
authorizationSystem
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphAuthorizationSystem
Parameter Sets: Update, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -DataCollectionInfo
dataCollectionInfo
To construct, see NOTES section for DATACOLLECTIONINFO properties and create a hash table.

```yaml
Type: IMicrosoftGraphDataCollectionInfo
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
Type: ISearchIdentity
Parameter Sets: UpdateViaIdentityExpanded, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
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

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphAuthorizationSystem
### Microsoft.Graph.Beta.PowerShell.Models.ISearchIdentity
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphAuthorizationSystem
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER \<IMicrosoftGraphAuthorizationSystem\>: authorizationSystem
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
  \[AuthorizationSystemId \<String\>\]: 
  \[AuthorizationSystemName \<String\>\]: 
  \[AuthorizationSystemType \<String\>\]: 
  \[DataCollectionInfo \<IMicrosoftGraphDataCollectionInfo\>\]: dataCollectionInfo
    \[(Any) \<Object\>\]: This indicates any property can be added to this object.
    \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
    \[Entitlements \<IMicrosoftGraphEntitlementsDataCollectionInfo\>\]: entitlementsDataCollectionInfo
      \[(Any) \<Object\>\]: This indicates any property can be added to this object.

DATACOLLECTIONINFO \<IMicrosoftGraphDataCollectionInfo\>: dataCollectionInfo
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
  \[Entitlements \<IMicrosoftGraphEntitlementsDataCollectionInfo\>\]: entitlementsDataCollectionInfo
    \[(Any) \<Object\>\]: This indicates any property can be added to this object.

INPUTOBJECT \<ISearchIdentity\>: Identity Parameter
  \[AcronymId \<String\>\]: The unique identifier of acronym
  \[AuthorizationSystemId \<String\>\]: The unique identifier of authorizationSystem
  \[BookmarkId \<String\>\]: The unique identifier of bookmark
  \[ConnectionOperationId \<String\>\]: The unique identifier of connectionOperation
  \[ExternalActivityId \<String\>\]: The unique identifier of externalActivity
  \[ExternalConnectionId \<String\>\]: The unique identifier of externalConnection
  \[ExternalGroupId \<String\>\]: The unique identifier of externalGroup
  \[ExternalItemId \<String\>\]: The unique identifier of externalItem
  \[IdentityId \<String\>\]: The unique identifier of identity
  \[InboundFlowId \<String\>\]: The unique identifier of inboundFlow
  \[IndustryDataConnectorId \<String\>\]: The unique identifier of industryDataConnector
  \[IndustryDataRunActivityId \<String\>\]: The unique identifier of industryDataRunActivity
  \[IndustryDataRunId \<String\>\]: The unique identifier of industryDataRun
  \[LongRunningOperationId \<String\>\]: The unique identifier of longRunningOperation
  \[QnaId \<String\>\]: The unique identifier of qna
  \[ReferenceDefinitionId \<String\>\]: The unique identifier of referenceDefinition
  \[RoleGroupId \<String\>\]: The unique identifier of roleGroup
  \[SourceSystemDefinitionId \<String\>\]: The unique identifier of sourceSystemDefinition
  \[YearTimePeriodDefinitionId \<String\>\]: The unique identifier of yearTimePeriodDefinition

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.search/update-mgbetaexternalauthorizationsystem](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.search/update-mgbetaexternalauthorizationsystem)



