---
external help file: Microsoft.Graph.DirectoryObjects-help.xml
Module Name: Microsoft.Graph.DirectoryObjects
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.directoryobjects/update-mgdirectoryobject
schema: 2.0.0
---

# Update-MgDirectoryObject

## SYNOPSIS
Update entity in directoryObjects

> [!NOTE]
> To view the beta release of this cmdlet, view [Update-MgBetaDirectoryObject](/powershell/module/Microsoft.Graph.Beta.DirectoryObjects/Update-MgBetaDirectoryObject?view=graph-powershell-beta)

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgDirectoryObject -DirectoryObjectId <String> [-AdditionalProperties <Hashtable>]
 [-DeletedDateTime <DateTime>] [-Id <String>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Update
```
Update-MgDirectoryObject -DirectoryObjectId <String> -BodyParameter <IMicrosoftGraphDirectoryObject> [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentityExpanded
```
Update-MgDirectoryObject -InputObject <IDirectoryObjectsIdentity> [-AdditionalProperties <Hashtable>]
 [-DeletedDateTime <DateTime>] [-Id <String>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentity
```
Update-MgDirectoryObject -InputObject <IDirectoryObjectsIdentity>
 -BodyParameter <IMicrosoftGraphDirectoryObject> [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Update entity in directoryObjects

## EXAMPLES
### Example 1: Code snippet

```powershell
Import-Module Microsoft.Graph.DirectoryObjects

Get-MgDirectoryObject -DirectoryObjectId $directoryObjectId
```
This example shows how to use the Update-MgDirectoryObject Cmdlet.

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

### -BodyParameter
directoryObject
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphDirectoryObject
Parameter Sets: Update, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -DeletedDateTime
Date and time when this object was deleted.
Always null when the object hasn't been deleted.

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

### -DirectoryObjectId
The unique identifier of directoryObject

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
Type: IDirectoryObjectsIdentity
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

### Microsoft.Graph.PowerShell.Models.IDirectoryObjectsIdentity
### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphDirectoryObject
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphDirectoryObject
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER \<IMicrosoftGraphDirectoryObject\>: directoryObject
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
  \[DeletedDateTime \<DateTime?\>\]: Date and time when this object was deleted.
Always null when the object hasn't been deleted.

INPUTOBJECT \<IDirectoryObjectsIdentity\>: Identity Parameter
  \[DirectoryObjectId \<String\>\]: The unique identifier of directoryObject

## RELATED LINKS
[Update-MgBetaDirectoryObject](/powershell/module/Microsoft.Graph.Beta.DirectoryObjects/Update-MgBetaDirectoryObject?view=graph-powershell-beta)

[https://learn.microsoft.com/powershell/module/microsoft.graph.directoryobjects/update-mgdirectoryobject](https://learn.microsoft.com/powershell/module/microsoft.graph.directoryobjects/update-mgdirectoryobject)


