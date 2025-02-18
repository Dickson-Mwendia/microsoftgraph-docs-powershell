---
external help file: Microsoft.Graph.Beta.Users.Actions-help.xml
Module Name: Microsoft.Graph.Beta.Users.Actions
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.users.actions/invoke-mgbetagraphuserchat
schema: 2.0.0
ms.prod: microsoft-teams
---

# Invoke-MgBetaGraphUserChat

## SYNOPSIS
Unhide a chat for a user.
This API is available in the following national cloud deployments.

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [Invoke-MgGraphUserChat](/powershell/module/Microsoft.Graph.Users.Actions/Invoke-MgGraphUserChat?view=graph-powershell-1.0)

## SYNTAX

### GraphExpanded (Default)
```
Invoke-MgBetaGraphUserChat -ChatId <String> -UserId <String> [-AdditionalProperties <Hashtable>]
 [-TenantId <String>] [-User <IMicrosoftGraphTeamworkUserIdentity>] [-PassThru] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### Graph
```
Invoke-MgBetaGraphUserChat -ChatId <String> -UserId <String>
 -Body <IPathsFqm7NdUsersUserIdChatsChatIdMicrosoftGraphUnhideforuserPostRequestbodyContentApplicationJsonSchema>
 [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### GraphViaIdentityExpanded
```
Invoke-MgBetaGraphUserChat -InputObject <IUsersActionsIdentity> [-AdditionalProperties <Hashtable>]
 [-TenantId <String>] [-User <IMicrosoftGraphTeamworkUserIdentity>] [-PassThru] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### GraphViaIdentity
```
Invoke-MgBetaGraphUserChat -InputObject <IUsersActionsIdentity>
 -BodyParameter <IPathsFqm7NdUsersUserIdChatsChatIdMicrosoftGraphUnhideforuserPostRequestbodyContentApplicationJsonSchema>
 [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Unhide a chat for a user.
This API is available in the following national cloud deployments.

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: GraphExpanded, GraphViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Body
.
To construct, see NOTES section for BODY properties and create a hash table.

```yaml
Type: IPathsFqm7NdUsersUserIdChatsChatIdMicrosoftGraphUnhideforuserPostRequestbodyContentApplicationJsonSchema
Parameter Sets: Graph
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -BodyParameter
.
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IPathsFqm7NdUsersUserIdChatsChatIdMicrosoftGraphUnhideforuserPostRequestbodyContentApplicationJsonSchema
Parameter Sets: GraphViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -ChatId
The unique identifier of chat

```yaml
Type: String
Parameter Sets: GraphExpanded, Graph
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
Type: IUsersActionsIdentity
Parameter Sets: GraphViaIdentityExpanded, GraphViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -PassThru
Returns true when the command succeeds

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -TenantId
.

```yaml
Type: String
Parameter Sets: GraphExpanded, GraphViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -User
teamworkUserIdentity
To construct, see NOTES section for USER properties and create a hash table.

```yaml
Type: IMicrosoftGraphTeamworkUserIdentity
Parameter Sets: GraphExpanded, GraphViaIdentityExpanded
Aliases:

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
Parameter Sets: GraphExpanded, Graph
Aliases:

Required: True
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

### Microsoft.Graph.Beta.PowerShell.Models.IPathsFqm7NdUsersUserIdChatsChatIdMicrosoftGraphUnhideforuserPostRequestbodyContentApplicationJsonSchema
### Microsoft.Graph.Beta.PowerShell.Models.IUsersActionsIdentity
## OUTPUTS

### System.Boolean
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODY \<IPathsFqm7NdUsersUserIdChatsChatIdMicrosoftGraphUnhideforuserPostRequestbodyContentApplicationJsonSchema\>: .
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[TenantId \<String\>\]: 
  \[User \<IMicrosoftGraphTeamworkUserIdentity\>\]: teamworkUserIdentity
    \[(Any) \<Object\>\]: This indicates any property can be added to this object.
    \[DisplayName \<String\>\]: The display name of the identity.
This might not always be available or up to date.
For example, if a user changes their display name, the API might show the new value in a future response, but the items associated with the user won't show up as having changed when using delta.
    \[Id \<String\>\]: Unique identifier for the identity.
    \[UserIdentityType \<String\>\]: teamworkUserIdentityType

BODYPARAMETER \<IPathsFqm7NdUsersUserIdChatsChatIdMicrosoftGraphUnhideforuserPostRequestbodyContentApplicationJsonSchema\>: .
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[TenantId \<String\>\]: 
  \[User \<IMicrosoftGraphTeamworkUserIdentity\>\]: teamworkUserIdentity
    \[(Any) \<Object\>\]: This indicates any property can be added to this object.
    \[DisplayName \<String\>\]: The display name of the identity.
This might not always be available or up to date.
For example, if a user changes their display name, the API might show the new value in a future response, but the items associated with the user won't show up as having changed when using delta.
    \[Id \<String\>\]: Unique identifier for the identity.
    \[UserIdentityType \<String\>\]: teamworkUserIdentityType

INPUTOBJECT \<IUsersActionsIdentity\>: Identity Parameter
  \[AccessReviewInstanceId \<String\>\]: The unique identifier of accessReviewInstance
  \[AccessReviewStageId \<String\>\]: The unique identifier of accessReviewStage
  \[AppLogCollectionRequestId \<String\>\]: The unique identifier of appLogCollectionRequest
  \[AuthenticationMethodId \<String\>\]: The unique identifier of authenticationMethod
  \[CalendarId \<String\>\]: The unique identifier of calendar
  \[ChatId \<String\>\]: The unique identifier of chat
  \[ChatMessageId \<String\>\]: The unique identifier of chatMessage
  \[ChatMessageId1 \<String\>\]: The unique identifier of chatMessage
  \[CloudPcId \<String\>\]: The unique identifier of cloudPC
  \[ContentTypeId \<String\>\]: The unique identifier of contentType
  \[DeviceEnrollmentConfigurationId \<String\>\]: The unique identifier of deviceEnrollmentConfiguration
  \[DeviceLogCollectionResponseId \<String\>\]: The unique identifier of deviceLogCollectionResponse
  \[DocumentSetVersionId \<String\>\]: The unique identifier of documentSetVersion
  \[DriveId \<String\>\]: The unique identifier of drive
  \[DriveItemId \<String\>\]: The unique identifier of driveItem
  \[DriveItemVersionId \<String\>\]: The unique identifier of driveItemVersion
  \[EventId \<String\>\]: The unique identifier of event
  \[EventId1 \<String\>\]: The unique identifier of event
  \[ListItemId \<String\>\]: The unique identifier of listItem
  \[ListItemVersionId \<String\>\]: The unique identifier of listItemVersion
  \[MailFolderId \<String\>\]: The unique identifier of mailFolder
  \[MailFolderId1 \<String\>\]: The unique identifier of mailFolder
  \[ManagedDeviceId \<String\>\]: The unique identifier of managedDevice
  \[MessageId \<String\>\]: The unique identifier of message
  \[MobileAppTroubleshootingEventId \<String\>\]: The unique identifier of mobileAppTroubleshootingEvent
  \[NotebookId \<String\>\]: The unique identifier of notebook
  \[OnenotePageId \<String\>\]: The unique identifier of onenotePage
  \[OnenoteSectionId \<String\>\]: The unique identifier of onenoteSection
  \[OutlookTaskFolderId \<String\>\]: The unique identifier of outlookTaskFolder
  \[OutlookTaskGroupId \<String\>\]: The unique identifier of outlookTaskGroup
  \[OutlookTaskId \<String\>\]: The unique identifier of outlookTask
  \[PermissionId \<String\>\]: The unique identifier of permission
  \[PlannerPlanId \<String\>\]: The unique identifier of plannerPlan
  \[SensitivityLabelId \<String\>\]: The unique identifier of sensitivityLabel
  \[SubscriptionId \<String\>\]: The unique identifier of subscription
  \[TeamsAppInstallationId \<String\>\]: The unique identifier of teamsAppInstallation
  \[TodoTaskId \<String\>\]: The unique identifier of todoTask
  \[TodoTaskListId \<String\>\]: The unique identifier of todoTaskList
  \[UserId \<String\>\]: The unique identifier of user

USER \<IMicrosoftGraphTeamworkUserIdentity\>: teamworkUserIdentity
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[DisplayName \<String\>\]: The display name of the identity.
This might not always be available or up to date.
For example, if a user changes their display name, the API might show the new value in a future response, but the items associated with the user won't show up as having changed when using delta.
  \[Id \<String\>\]: Unique identifier for the identity.
  \[UserIdentityType \<String\>\]: teamworkUserIdentityType

## RELATED LINKS
[Invoke-MgGraphUserChat](/powershell/module/Microsoft.Graph.Users.Actions/Invoke-MgGraphUserChat?view=graph-powershell-1.0)

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.users.actions/invoke-mgbetagraphuserchat](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.users.actions/invoke-mgbetagraphuserchat)



