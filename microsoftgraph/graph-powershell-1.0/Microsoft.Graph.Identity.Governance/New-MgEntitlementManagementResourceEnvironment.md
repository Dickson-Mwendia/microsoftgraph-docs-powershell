---
external help file: Microsoft.Graph.Identity.Governance-help.xml
Module Name: Microsoft.Graph.Identity.Governance
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.identity.governance/new-mgentitlementmanagementresourceenvironment
schema: 2.0.0
---

# New-MgEntitlementManagementResourceEnvironment

## SYNOPSIS
Create new navigation property to resourceEnvironments for identityGovernance

## SYNTAX

### CreateExpanded (Default)
```
New-MgEntitlementManagementResourceEnvironment [-AdditionalProperties <Hashtable>]
 [-CreatedDateTime <DateTime>] [-Description <String>] [-DisplayName <String>] [-Id <String>]
 [-IsDefaultEnvironment] [-ModifiedDateTime <DateTime>] [-OriginId <String>] [-OriginSystem <String>]
 [-Resources <IMicrosoftGraphAccessPackageResource[]>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgEntitlementManagementResourceEnvironment -BodyParameter <IMicrosoftGraphAccessPackageResourceEnvironment>
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create new navigation property to resourceEnvironments for identityGovernance

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

### -BodyParameter
accessPackageResourceEnvironment
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphAccessPackageResourceEnvironment
Parameter Sets: Create
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -CreatedDateTime
The date and time that this object was created.
The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.

```yaml
Type: DateTime
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Description
The description of this object.

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

### -DisplayName
The display name of this object.

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

### -IsDefaultEnvironment
Determines whether this is default environment or not.
It is set to true for all static origin systems, such as Microsoft Entra groups and Microsoft Entra Applications.

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

### -ModifiedDateTime
The date and time that this object was last modified.
The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.

```yaml
Type: DateTime
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -OriginId
The unique identifier of this environment in the origin system.

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

### -OriginSystem
The type of the resource in the origin system, that is, SharePointOnline.
Requires $filter (eq).

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

### -Resources
Read-only.
Required.
To construct, see NOTES section for RESOURCES properties and create a hash table.

```yaml
Type: IMicrosoftGraphAccessPackageResource[]
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

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphAccessPackageResourceEnvironment
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphAccessPackageResourceEnvironment
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER \<IMicrosoftGraphAccessPackageResourceEnvironment\>: accessPackageResourceEnvironment
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
    \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
    \[CreatedDateTime \<DateTime?\>\]: The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Read-only.
    \[Description \<String\>\]: A description for the resource.
    \[DisplayName \<String\>\]: The display name of the resource, such as the application name, group name or site name.
    \[Environment \<IMicrosoftGraphAccessPackageResourceEnvironment\>\]: accessPackageResourceEnvironment
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
      \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
      \[Description \<String\>\]: The description of the scope.
      \[DisplayName \<String\>\]: The display name of the scope.
      \[IsRootScope \<Boolean?\>\]: True if the scopes are arranged in a hierarchy and this is the top or root scope of the resource.
      \[OriginId \<String\>\]: The unique identifier for the scope in the resource as defined in the origin system.
      \[OriginSystem \<String\>\]: The origin system for the scope.
      \[Resource \<IMicrosoftGraphAccessPackageResource\>\]: accessPackageResource

RESOURCES \<IMicrosoftGraphAccessPackageResource\[\]\>: Read-only.
Required.
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
    \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
    \[Description \<String\>\]: The description of the scope.
    \[DisplayName \<String\>\]: The display name of the scope.
    \[IsRootScope \<Boolean?\>\]: True if the scopes are arranged in a hierarchy and this is the top or root scope of the resource.
    \[OriginId \<String\>\]: The unique identifier for the scope in the resource as defined in the origin system.
    \[OriginSystem \<String\>\]: The origin system for the scope.
    \[Resource \<IMicrosoftGraphAccessPackageResource\>\]: accessPackageResource

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.identity.governance/new-mgentitlementmanagementresourceenvironment](https://learn.microsoft.com/powershell/module/microsoft.graph.identity.governance/new-mgentitlementmanagementresourceenvironment)


