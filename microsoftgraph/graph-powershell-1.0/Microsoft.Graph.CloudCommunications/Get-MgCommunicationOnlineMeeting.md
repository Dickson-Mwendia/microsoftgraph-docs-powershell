---
external help file: Microsoft.Graph.CloudCommunications-help.xml
Module Name: Microsoft.Graph.CloudCommunications
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.cloudcommunications/get-mgcommunicationonlinemeeting
schema: 2.0.0
ms.prod: cloud-communications
---

# Get-MgCommunicationOnlineMeeting

## SYNOPSIS
Get onlineMeetings from communications

> [!NOTE]
> To view the beta release of this cmdlet, view [Get-MgBetaCommunicationOnlineMeeting](/powershell/module/Microsoft.Graph.Beta.CloudCommunications/Get-MgBetaCommunicationOnlineMeeting?view=graph-powershell-beta)

## SYNTAX

### GetExpanded (Default)
```
Get-MgCommunicationOnlineMeeting [-AdditionalProperties <Hashtable>] [-ChatInfo <IMicrosoftGraphChatInfo>]
 [-EndDateTime <DateTime>] [-ExternalId <String>] [-Participants <IMicrosoftGraphMeetingParticipants>]
 [-StartDateTime <DateTime>] [-Subject <String>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Get
```
Get-MgCommunicationOnlineMeeting -OnlineMeetingId <String> [-ExpandProperty <String[]>] [-Property <String[]>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### GetViaIdentity
```
Get-MgCommunicationOnlineMeeting -InputObject <ICloudCommunicationsIdentity> [-ExpandProperty <String[]>]
 [-Property <String[]>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### List
```
Get-MgCommunicationOnlineMeeting [-ExpandProperty <String[]>] [-Property <String[]>] [-Filter <String>]
 [-Search <String>] [-Skip <Int32>] [-Sort <String[]>] [-Top <Int32>] [-PageSize <Int32>] [-All]
 [-CountVariable <String>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Get1
```
Get-MgCommunicationOnlineMeeting
 -BodyParameter <IPaths1Pc6SxrCommunicationsOnlinemeetingsMicrosoftGraphCreateorgetPostRequestbodyContentApplicationJsonSchema>
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Get onlineMeetings from communications

## EXAMPLES
### Example 1: Retrieve an online meeting by videoTeleconferenceId

```powershell

Import-Module Microsoft.Graph.CloudCommunications

Get-MgCommunicationOnlineMeeting -Filter "VideoTeleconferenceId eq '123456789'" 

```
This example will retrieve an online meeting by videoteleconferenceid


## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: GetExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -All
List all pages.

```yaml
Type: SwitchParameter
Parameter Sets: List
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
.
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IPaths1Pc6SxrCommunicationsOnlinemeetingsMicrosoftGraphCreateorgetPostRequestbodyContentApplicationJsonSchema
Parameter Sets: Get1
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -ChatInfo
chatInfo
To construct, see NOTES section for CHATINFO properties and create a hash table.

```yaml
Type: IMicrosoftGraphChatInfo
Parameter Sets: GetExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CountVariable
Specifies a count of the total number of items in a collection.
By default, this variable will be set in the global scope.

```yaml
Type: String
Parameter Sets: List
Aliases: CV

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -EndDateTime
.

```yaml
Type: DateTime
Parameter Sets: GetExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ExpandProperty
Expand related entities

```yaml
Type: String[]
Parameter Sets: Get, GetViaIdentity, List
Aliases: Expand

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ExternalId
.

```yaml
Type: String
Parameter Sets: GetExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Filter
Filter items by property values

```yaml
Type: String
Parameter Sets: List
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
Type: ICloudCommunicationsIdentity
Parameter Sets: GetViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -OnlineMeetingId
The unique identifier of onlineMeeting

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

### -PageSize
Sets the page size of results.

```yaml
Type: Int32
Parameter Sets: List
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -Participants
meetingParticipants
To construct, see NOTES section for PARTICIPANTS properties and create a hash table.

```yaml
Type: IMicrosoftGraphMeetingParticipants
Parameter Sets: GetExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Property
Select properties to be returned

```yaml
Type: String[]
Parameter Sets: Get, GetViaIdentity, List
Aliases: Select

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Search
Search items by search phrases

```yaml
Type: String
Parameter Sets: List
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Sort
Order items by property values

```yaml
Type: String[]
Parameter Sets: List
Aliases: OrderBy

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -StartDateTime
.

```yaml
Type: DateTime
Parameter Sets: GetExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Subject
.

```yaml
Type: String
Parameter Sets: GetExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Top
Show only the first n items

```yaml
Type: Int32
Parameter Sets: List
Aliases: Limit

Required: False
Position: Named
Default value: 0
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

### -Skip
Skip the first n items

```yaml
Type: Int32
Parameter Sets: List
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.Graph.PowerShell.Models.ICloudCommunicationsIdentity
### Microsoft.Graph.PowerShell.Models.IPaths1Pc6SxrCommunicationsOnlinemeetingsMicrosoftGraphCreateorgetPostRequestbodyContentApplicationJsonSchema
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphOnlineMeeting
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER \<IPaths1Pc6SxrCommunicationsOnlinemeetingsMicrosoftGraphCreateorgetPostRequestbodyContentApplicationJsonSchema\>: .
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[ChatInfo \<IMicrosoftGraphChatInfo\>\]: chatInfo
    \[(Any) \<Object\>\]: This indicates any property can be added to this object.
    \[MessageId \<String\>\]: The unique identifier of a message in a Microsoft Teams channel.
    \[ReplyChainMessageId \<String\>\]: The ID of the reply message.
    \[ThreadId \<String\>\]: The unique identifier for a thread in Microsoft Teams.
  \[EndDateTime \<DateTime?\>\]: 
  \[ExternalId \<String\>\]: 
  \[Participants \<IMicrosoftGraphMeetingParticipants\>\]: meetingParticipants
    \[(Any) \<Object\>\]: This indicates any property can be added to this object.
    \[Attendees \<IMicrosoftGraphMeetingParticipantInfo\[\]\>\]: 
      \[Identity \<IMicrosoftGraphIdentitySet\>\]: identitySet
        \[(Any) \<Object\>\]: This indicates any property can be added to this object.
        \[Application \<IMicrosoftGraphIdentity\>\]: identity
          \[(Any) \<Object\>\]: This indicates any property can be added to this object.
          \[DisplayName \<String\>\]: The display name of the identity.
The display name might not always be available or up to date.
For example, if a user changes their display name, the API might show the new value in a future response, but the items associated with the user won't show up as having changed when using delta.
          \[Id \<String\>\]: Unique identifier for the identity.
        \[Device \<IMicrosoftGraphIdentity\>\]: identity
        \[User \<IMicrosoftGraphIdentity\>\]: identity
      \[Role \<String\>\]: onlineMeetingRole
      \[Upn \<String\>\]: User principal name of the participant.
    \[Organizer \<IMicrosoftGraphMeetingParticipantInfo\>\]: meetingParticipantInfo
  \[StartDateTime \<DateTime?\>\]: 
  \[Subject \<String\>\]: 

CHATINFO \<IMicrosoftGraphChatInfo\>: chatInfo
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[MessageId \<String\>\]: The unique identifier of a message in a Microsoft Teams channel.
  \[ReplyChainMessageId \<String\>\]: The ID of the reply message.
  \[ThreadId \<String\>\]: The unique identifier for a thread in Microsoft Teams.

INPUTOBJECT \<ICloudCommunicationsIdentity\>: Identity Parameter
  \[AttendanceRecordId \<String\>\]: The unique identifier of attendanceRecord
  \[AudioRoutingGroupId \<String\>\]: The unique identifier of audioRoutingGroup
  \[CallId \<String\>\]: The unique identifier of call
  \[CallRecordId \<String\>\]: The unique identifier of callRecord
  \[CallTranscriptId \<String\>\]: The unique identifier of callTranscript
  \[CommsOperationId \<String\>\]: The unique identifier of commsOperation
  \[ContentSharingSessionId \<String\>\]: The unique identifier of contentSharingSession
  \[MeetingAttendanceReportId \<String\>\]: The unique identifier of meetingAttendanceReport
  \[OnlineMeetingId \<String\>\]: The unique identifier of onlineMeeting
  \[ParticipantId \<String\>\]: The unique identifier of participant
  \[PresenceId \<String\>\]: The unique identifier of presence
  \[SessionId \<String\>\]: The unique identifier of session
  \[UserId \<String\>\]: The unique identifier of user

PARTICIPANTS \<IMicrosoftGraphMeetingParticipants\>: meetingParticipants
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[Attendees \<IMicrosoftGraphMeetingParticipantInfo\[\]\>\]: 
    \[Identity \<IMicrosoftGraphIdentitySet\>\]: identitySet
      \[(Any) \<Object\>\]: This indicates any property can be added to this object.
      \[Application \<IMicrosoftGraphIdentity\>\]: identity
        \[(Any) \<Object\>\]: This indicates any property can be added to this object.
        \[DisplayName \<String\>\]: The display name of the identity.
The display name might not always be available or up to date.
For example, if a user changes their display name, the API might show the new value in a future response, but the items associated with the user won't show up as having changed when using delta.
        \[Id \<String\>\]: Unique identifier for the identity.
      \[Device \<IMicrosoftGraphIdentity\>\]: identity
      \[User \<IMicrosoftGraphIdentity\>\]: identity
    \[Role \<String\>\]: onlineMeetingRole
    \[Upn \<String\>\]: User principal name of the participant.
  \[Organizer \<IMicrosoftGraphMeetingParticipantInfo\>\]: meetingParticipantInfo

## RELATED LINKS
[Get-MgBetaCommunicationOnlineMeeting](/powershell/module/Microsoft.Graph.Beta.CloudCommunications/Get-MgBetaCommunicationOnlineMeeting?view=graph-powershell-beta)

[https://learn.microsoft.com/powershell/module/microsoft.graph.cloudcommunications/get-mgcommunicationonlinemeeting](https://learn.microsoft.com/powershell/module/microsoft.graph.cloudcommunications/get-mgcommunicationonlinemeeting)


