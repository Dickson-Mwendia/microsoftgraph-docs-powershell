---
external help file: Microsoft.Graph.Beta.Bookings-help.xml
Module Name: Microsoft.Graph.Beta.Bookings
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.bookings/update-mgbetavirtualeventwebinarsessionregistration
schema: 2.0.0
ms.prod: cloud-communications
---

# Update-MgBetaVirtualEventWebinarSessionRegistration

## SYNOPSIS
Update the details of a meetingRegistration object assciated with an onlineMeeting on behalf of the organizer.
This API is available in the following national cloud deployments.

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgBetaVirtualEventWebinarSessionRegistration -VirtualEventSessionId <String>
 -VirtualEventWebinarId <String> [-AdditionalProperties <Hashtable>] [-AllowedRegistrant <String>]
 [-CustomQuestions <IMicrosoftGraphMeetingRegistrationQuestion[]>] [-Description <String>]
 [-EndDateTime <DateTime>] [-Id <String>] [-Registrants <IMicrosoftGraphMeetingRegistrantBase[]>]
 [-RegistrationPageViewCount <Int32>] [-RegistrationPageWebUrl <String>]
 [-Speakers <IMicrosoftGraphMeetingSpeaker[]>] [-StartDateTime <DateTime>] [-Subject <String>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### Update
```
Update-MgBetaVirtualEventWebinarSessionRegistration -VirtualEventSessionId <String>
 -VirtualEventWebinarId <String> -BodyParameter <IMicrosoftGraphMeetingRegistration> [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### UpdateViaIdentityExpanded
```
Update-MgBetaVirtualEventWebinarSessionRegistration -InputObject <IBookingsIdentity>
 [-AdditionalProperties <Hashtable>] [-AllowedRegistrant <String>]
 [-CustomQuestions <IMicrosoftGraphMeetingRegistrationQuestion[]>] [-Description <String>]
 [-EndDateTime <DateTime>] [-Id <String>] [-Registrants <IMicrosoftGraphMeetingRegistrantBase[]>]
 [-RegistrationPageViewCount <Int32>] [-RegistrationPageWebUrl <String>]
 [-Speakers <IMicrosoftGraphMeetingSpeaker[]>] [-StartDateTime <DateTime>] [-Subject <String>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentity
```
Update-MgBetaVirtualEventWebinarSessionRegistration -InputObject <IBookingsIdentity>
 -BodyParameter <IMicrosoftGraphMeetingRegistration> [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Update the details of a meetingRegistration object assciated with an onlineMeeting on behalf of the organizer.
This API is available in the following national cloud deployments.

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

### -AllowedRegistrant
meetingAudience

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
meetingRegistration
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphMeetingRegistration
Parameter Sets: Update, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -CustomQuestions
Custom registration questions.
To construct, see NOTES section for CUSTOMQUESTIONS properties and create a hash table.

```yaml
Type: IMicrosoftGraphMeetingRegistrationQuestion[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Description
The description of the meeting.

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

### -EndDateTime
The meeting end time in UTC.

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
Type: IBookingsIdentity
Parameter Sets: UpdateViaIdentityExpanded, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Registrants
Registrants of the online meeting.
To construct, see NOTES section for REGISTRANTS properties and create a hash table.

```yaml
Type: IMicrosoftGraphMeetingRegistrantBase[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RegistrationPageViewCount
The number of times the registration page has been visited.
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

### -RegistrationPageWebUrl
The URL of the registration page.
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

### -Speakers
The meeting speaker's information.
To construct, see NOTES section for SPEAKERS properties and create a hash table.

```yaml
Type: IMicrosoftGraphMeetingSpeaker[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -StartDateTime
The meeting start time in UTC.

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

### -Subject
The subject of the meeting.

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

### -VirtualEventSessionId
The unique identifier of virtualEventSession

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

### -VirtualEventWebinarId
The unique identifier of virtualEventWebinar

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

### Microsoft.Graph.Beta.PowerShell.Models.IBookingsIdentity
### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphMeetingRegistration
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphMeetingRegistration
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER \<IMicrosoftGraphMeetingRegistration\>: meetingRegistration
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[AllowedRegistrant \<String\>\]: meetingAudience
  \[Registrants \<IMicrosoftGraphMeetingRegistrantBase\[\]\>\]: Registrants of the online meeting.
    \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
    \[JoinWebUrl \<String\>\]: A unique web URL for the registrant to join the meeting.
Read-only.
  \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
  \[CustomQuestions \<IMicrosoftGraphMeetingRegistrationQuestion\[\]\>\]: Custom registration questions.
    \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
    \[AnswerInputType \<String\>\]: answerInputType
    \[AnswerOptions \<String\[\]\>\]: Answer options when answerInputType is radioButton.
    \[DisplayName \<String\>\]: Display name of the custom registration question.
    \[IsRequired \<Boolean?\>\]: Indicates whether the question is required.
Default value is false.
  \[Description \<String\>\]: The description of the meeting.
  \[EndDateTime \<DateTime?\>\]: The meeting end time in UTC.
  \[RegistrationPageViewCount \<Int32?\>\]: The number of times the registration page has been visited.
Read-only.
  \[RegistrationPageWebUrl \<String\>\]: The URL of the registration page.
Read-only.
  \[Speakers \<IMicrosoftGraphMeetingSpeaker\[\]\>\]: The meeting speaker's information.
    \[Bio \<String\>\]: Bio of the speaker.
    \[DisplayName \<String\>\]: Display name of the speaker.
  \[StartDateTime \<DateTime?\>\]: The meeting start time in UTC.
  \[Subject \<String\>\]: The subject of the meeting.

CUSTOMQUESTIONS \<IMicrosoftGraphMeetingRegistrationQuestion\[\]\>: Custom registration questions.
  \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
  \[AnswerInputType \<String\>\]: answerInputType
  \[AnswerOptions \<String\[\]\>\]: Answer options when answerInputType is radioButton.
  \[DisplayName \<String\>\]: Display name of the custom registration question.
  \[IsRequired \<Boolean?\>\]: Indicates whether the question is required.
Default value is false.

INPUTOBJECT \<IBookingsIdentity\>: Identity Parameter
  \[AttendanceRecordId \<String\>\]: The unique identifier of attendanceRecord
  \[BookingAppointmentId \<String\>\]: The unique identifier of bookingAppointment
  \[BookingBusinessId \<String\>\]: The unique identifier of bookingBusiness
  \[BookingCurrencyId \<String\>\]: The unique identifier of bookingCurrency
  \[BookingCustomQuestionId \<String\>\]: The unique identifier of bookingCustomQuestion
  \[BookingCustomerId \<String\>\]: The unique identifier of bookingCustomer
  \[BookingServiceId \<String\>\]: The unique identifier of bookingService
  \[BookingStaffMemberId \<String\>\]: The unique identifier of bookingStaffMember
  \[BusinessScenarioId \<String\>\]: The unique identifier of businessScenario
  \[BusinessScenarioTaskId \<String\>\]: The unique identifier of businessScenarioTask
  \[CallRecordingId \<String\>\]: The unique identifier of callRecording
  \[CallTranscriptId \<String\>\]: The unique identifier of callTranscript
  \[MeetingAttendanceReportId \<String\>\]: The unique identifier of meetingAttendanceReport
  \[MeetingRegistrantBaseId \<String\>\]: The unique identifier of meetingRegistrantBase
  \[MeetingRegistrationQuestionId \<String\>\]: The unique identifier of meetingRegistrationQuestion
  \[PlannerPlanConfigurationLocalizationId \<String\>\]: The unique identifier of plannerPlanConfigurationLocalization
  \[Role \<String\>\]: Usage: role='{role}'
  \[UserId \<String\>\]: Usage: userId='{userId}'
  \[VirtualEventId \<String\>\]: The unique identifier of virtualEvent
  \[VirtualEventPresenterId \<String\>\]: The unique identifier of virtualEventPresenter
  \[VirtualEventRegistrationId \<String\>\]: The unique identifier of virtualEventRegistration
  \[VirtualEventSessionId \<String\>\]: The unique identifier of virtualEventSession
  \[VirtualEventWebinarId \<String\>\]: The unique identifier of virtualEventWebinar

REGISTRANTS \<IMicrosoftGraphMeetingRegistrantBase\[\]\>: Registrants of the online meeting.
  \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
  \[JoinWebUrl \<String\>\]: A unique web URL for the registrant to join the meeting.
Read-only.

SPEAKERS \<IMicrosoftGraphMeetingSpeaker\[\]\>: The meeting speaker's information.
  \[Bio \<String\>\]: Bio of the speaker.
  \[DisplayName \<String\>\]: Display name of the speaker.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.bookings/update-mgbetavirtualeventwebinarsessionregistration](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.bookings/update-mgbetavirtualeventwebinarsessionregistration)


