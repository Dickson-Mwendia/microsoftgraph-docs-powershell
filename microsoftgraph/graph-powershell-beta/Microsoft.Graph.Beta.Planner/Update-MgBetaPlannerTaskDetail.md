---
external help file: Microsoft.Graph.Beta.Planner-help.xml
Module Name: Microsoft.Graph.Beta.Planner
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.planner/update-mgbetaplannertaskdetail
schema: 2.0.0
ms.prod: planner
---

# Update-MgBetaPlannerTaskDetail

## SYNOPSIS
Update the navigation property details in planner

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [Update-MgPlannerTaskDetail](/powershell/module/Microsoft.Graph.Planner/Update-MgPlannerTaskDetail?view=graph-powershell-1.0)

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgBetaPlannerTaskDetail -PlannerTaskId <String> -IfMatch <String> [-AdditionalProperties <Hashtable>]
 [-Checklist <Hashtable>] [-CompletionRequirements <IMicrosoftGraphPlannerTaskCompletionRequirementDetails>]
 [-Description <String>] [-Id <String>] [-Notes <IMicrosoftGraphItemBody>] [-PreviewType <String>]
 [-References <Hashtable>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Update
```
Update-MgBetaPlannerTaskDetail -PlannerTaskId <String> -IfMatch <String>
 -BodyParameter <IMicrosoftGraphPlannerTaskDetails> [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentityExpanded
```
Update-MgBetaPlannerTaskDetail -InputObject <IPlannerIdentity> -IfMatch <String>
 [-AdditionalProperties <Hashtable>] [-Checklist <Hashtable>]
 [-CompletionRequirements <IMicrosoftGraphPlannerTaskCompletionRequirementDetails>] [-Description <String>]
 [-Id <String>] [-Notes <IMicrosoftGraphItemBody>] [-PreviewType <String>] [-References <Hashtable>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentity
```
Update-MgBetaPlannerTaskDetail -InputObject <IPlannerIdentity> -IfMatch <String>
 -BodyParameter <IMicrosoftGraphPlannerTaskDetails> [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Update the navigation property details in planner

## EXAMPLES
### Example 1: Code snippet

```powershell
Import-Module Microsoft.Graph.Beta.Planner

$params = @{
	previewType = "noPreview"
	references = @{
		"http%3A//developer%2Emicrosoft%2Ecom" = @{
			"@odata.type" = "microsoft.graph.plannerExternalReference"
			alias = "Documentation"
			previewPriority = " !"
			type = "Other"
		}
		"https%3A//developer%2Emicrosoft%2Ecom/graph/graph-explorer" = @{
			"@odata.type" = "microsoft.graph.plannerExternalReference"
			previewPriority = "  !!"
		}
		"http%3A//www%2Ebing%2Ecom" = $null
	}
	checklist = @{
		"95e27074-6c4a-447a-aa24-9d718a0b86fa" = @{
			"@odata.type" = "microsoft.graph.plannerChecklistItem"
			title = "Update task details"
			isChecked = $true
		}
		"d280ed1a-9f6b-4f9c-a962-fb4d00dc50ff" = @{
			"@odata.type" = "microsoft.graph.plannerChecklistItem"
			isChecked = $true
		}
		"a93c93c5-10a6-4167-9551-8bafa09967a7" = $null
	}
	description = "Updated task details properties:
Updated checklist:Sub items
Updated references:Related links"
}

Update-MgBetaPlannerTaskDetail -PlannerTaskId $plannerTaskId -BodyParameter $params-If-Match W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="
```
This example shows how to use the Update-MgBetaPlannerTaskDetail Cmdlet.

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
plannerTaskDetails
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphPlannerTaskDetails
Parameter Sets: Update, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Checklist
plannerChecklistItems

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

### -CompletionRequirements
plannerTaskCompletionRequirementDetails
To construct, see NOTES section for COMPLETIONREQUIREMENTS properties and create a hash table.

```yaml
Type: IMicrosoftGraphPlannerTaskCompletionRequirementDetails
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Description
Description of the task.

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

### -IfMatch
ETag value.

```yaml
Type: String
Parameter Sets: (All)
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
Type: IPlannerIdentity
Parameter Sets: UpdateViaIdentityExpanded, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Notes
itemBody
To construct, see NOTES section for NOTES properties and create a hash table.

```yaml
Type: IMicrosoftGraphItemBody
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PlannerTaskId
The unique identifier of plannerTask

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

### -PreviewType
plannerPreviewType

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

### -References
plannerExternalReferences

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

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphPlannerTaskDetails
### Microsoft.Graph.Beta.PowerShell.Models.IPlannerIdentity
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphPlannerTaskDetails
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER \<IMicrosoftGraphPlannerTaskDetails\>: plannerTaskDetails
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
  \[Checklist \<IMicrosoftGraphPlannerChecklistItems\>\]: plannerChecklistItems
    \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[CompletionRequirements \<IMicrosoftGraphPlannerTaskCompletionRequirementDetails\>\]: plannerTaskCompletionRequirementDetails
    \[(Any) \<Object\>\]: This indicates any property can be added to this object.
    \[ChecklistRequirement \<IMicrosoftGraphPlannerChecklistRequirement\>\]: plannerChecklistRequirement
      \[(Any) \<Object\>\]: This indicates any property can be added to this object.
      \[RequiredChecklistItemIds \<String\[\]\>\]: A collection of required plannerChecklistItems identifiers to complete the plannerTask.
  \[Description \<String\>\]: Description of the task.
  \[Notes \<IMicrosoftGraphItemBody\>\]: itemBody
    \[(Any) \<Object\>\]: This indicates any property can be added to this object.
    \[Content \<String\>\]: The content of the item.
    \[ContentType \<String\>\]: bodyType
  \[PreviewType \<String\>\]: plannerPreviewType
  \[References \<IMicrosoftGraphPlannerExternalReferences\>\]: plannerExternalReferences
    \[(Any) \<Object\>\]: This indicates any property can be added to this object.

COMPLETIONREQUIREMENTS \<IMicrosoftGraphPlannerTaskCompletionRequirementDetails\>: plannerTaskCompletionRequirementDetails
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[ChecklistRequirement \<IMicrosoftGraphPlannerChecklistRequirement\>\]: plannerChecklistRequirement
    \[(Any) \<Object\>\]: This indicates any property can be added to this object.
    \[RequiredChecklistItemIds \<String\[\]\>\]: A collection of required plannerChecklistItems identifiers to complete the plannerTask.

INPUTOBJECT \<IPlannerIdentity\>: Identity Parameter
  \[GroupId \<String\>\]: The unique identifier of group
  \[PlannerBucketId \<String\>\]: The unique identifier of plannerBucket
  \[PlannerDeltaId \<String\>\]: The unique identifier of plannerDelta
  \[PlannerPlanId \<String\>\]: The unique identifier of plannerPlan
  \[PlannerRosterId \<String\>\]: The unique identifier of plannerRoster
  \[PlannerRosterMemberId \<String\>\]: The unique identifier of plannerRosterMember
  \[PlannerTaskId \<String\>\]: The unique identifier of plannerTask
  \[UserId \<String\>\]: The unique identifier of user

NOTES \<IMicrosoftGraphItemBody\>: itemBody
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[Content \<String\>\]: The content of the item.
  \[ContentType \<String\>\]: bodyType

## RELATED LINKS
[Update-MgPlannerTaskDetail](/powershell/module/Microsoft.Graph.Planner/Update-MgPlannerTaskDetail?view=graph-powershell-1.0)

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.planner/update-mgbetaplannertaskdetail](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.planner/update-mgbetaplannertaskdetail)


