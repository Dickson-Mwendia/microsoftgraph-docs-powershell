---
external help file: Microsoft.Graph.PersonalContacts-help.xml
Module Name: Microsoft.Graph.PersonalContacts
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.personalcontacts/get-mgusercontactfoldercontactphoto
schema: 2.0.0
---

# Get-MgUserContactFolderContactPhoto

## SYNOPSIS
Optional contact picture.
You can get or set a photo for a contact.

> [!NOTE]
> To view the beta release of this cmdlet, view [Get-MgBetaUserContactFolderContactPhoto](/powershell/module/Microsoft.Graph.Beta.PersonalContacts/Get-MgBetaUserContactFolderContactPhoto?view=graph-powershell-beta)

## SYNTAX

### Get (Default)
```
Get-MgUserContactFolderContactPhoto -ContactFolderId <String> -ContactId <String> -UserId <String>
 [-Property <String[]>] [<CommonParameters>]
```

### GetViaIdentity
```
Get-MgUserContactFolderContactPhoto -InputObject <IPersonalContactsIdentity> [-Property <String[]>]
 [<CommonParameters>]
```

## DESCRIPTION
Optional contact picture.
You can get or set a photo for a contact.

## PARAMETERS

### -ContactFolderId
The unique identifier of contactFolder

```yaml
Type: String
Parameter Sets: Get
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ContactId
The unique identifier of contact

```yaml
Type: String
Parameter Sets: Get
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InputObject
Identity Parameter
To construct, see NOTES section for INPUTOBJECT properties and create a hash table.

```yaml
Type: IPersonalContactsIdentity
Parameter Sets: GetViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Property
Select properties to be returned

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: Select

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -UserId
The unique identifier of user

```yaml
Type: String
Parameter Sets: Get
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.Graph.PowerShell.Models.IPersonalContactsIdentity
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphProfilePhoto
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

INPUTOBJECT \<IPersonalContactsIdentity\>: Identity Parameter
  \[ContactFolderId \<String\>\]: The unique identifier of contactFolder
  \[ContactFolderId1 \<String\>\]: The unique identifier of contactFolder
  \[ContactId \<String\>\]: The unique identifier of contact
  \[ExtensionId \<String\>\]: The unique identifier of extension
  \[UserId \<String\>\]: The unique identifier of user

## RELATED LINKS
[Get-MgBetaUserContactFolderContactPhoto](/powershell/module/Microsoft.Graph.Beta.PersonalContacts/Get-MgBetaUserContactFolderContactPhoto?view=graph-powershell-beta)

[https://learn.microsoft.com/powershell/module/microsoft.graph.personalcontacts/get-mgusercontactfoldercontactphoto](https://learn.microsoft.com/powershell/module/microsoft.graph.personalcontacts/get-mgusercontactfoldercontactphoto)



