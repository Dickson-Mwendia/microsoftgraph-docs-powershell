---
external help file: Microsoft.Graph.Beta.DeviceManagement-help.xml
Module Name: Microsoft.Graph.Beta.DeviceManagement
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.devicemanagement/new-mgbetadevicemanagementuserexperienceanalyticbatteryhealthappimpact
schema: 2.0.0
---

# New-MgBetaDeviceManagementUserExperienceAnalyticBatteryHealthAppImpact

## SYNOPSIS
Create new navigation property to userExperienceAnalyticsBatteryHealthAppImpact for deviceManagement

## SYNTAX

### CreateExpanded (Default)
```
New-MgBetaDeviceManagementUserExperienceAnalyticBatteryHealthAppImpact [-ActiveDevices <Int32>]
 [-AdditionalProperties <Hashtable>] [-AppDisplayName <String>] [-AppName <String>] [-AppPublisher <String>]
 [-BatteryUsagePercentage <Double>] [-Id <String>] [-IsForegroundApp] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgBetaDeviceManagementUserExperienceAnalyticBatteryHealthAppImpact
 -BodyParameter <IMicrosoftGraphUserExperienceAnalyticsBatteryHealthAppImpact> [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

## DESCRIPTION
Create new navigation property to userExperienceAnalyticsBatteryHealthAppImpact for deviceManagement

## PARAMETERS

### -ActiveDevices
Number of active devices for using that app over a 14-day period.
Valid values 0 to 2147483647

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

### -AppDisplayName
User friendly display name for the app.
Eg: Outlook

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

### -AppName
App name.
Eg: oltk.exe

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

### -AppPublisher
App publisher.
Eg: Microsoft Corporation

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

### -BatteryUsagePercentage
The percent of total battery power used by this application when the device was not plugged into AC power, over 14 days computed across all devices in the tenant.
Unit in percentage.
Valid values 0 to 1.79769313486232E+308

```yaml
Type: Double
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
The user experience analytics battery health app impact entity contains battery usage related information at an app level for the tenant.
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphUserExperienceAnalyticsBatteryHealthAppImpact
Parameter Sets: Create
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
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

### -IsForegroundApp
true if the user had active interaction with the app.

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

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphUserExperienceAnalyticsBatteryHealthAppImpact
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphUserExperienceAnalyticsBatteryHealthAppImpact
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER \<IMicrosoftGraphUserExperienceAnalyticsBatteryHealthAppImpact\>: The user experience analytics battery health app impact entity contains battery usage related information at an app level for the tenant.
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
  \[ActiveDevices \<Int32?\>\]: Number of active devices for using that app over a 14-day period.
Valid values 0 to 2147483647
  \[AppDisplayName \<String\>\]: User friendly display name for the app.
Eg: Outlook
  \[AppName \<String\>\]: App name.
Eg: oltk.exe
  \[AppPublisher \<String\>\]: App publisher.
Eg: Microsoft Corporation
  \[BatteryUsagePercentage \<Double?\>\]: The percent of total battery power used by this application when the device was not plugged into AC power, over 14 days computed across all devices in the tenant.
Unit in percentage.
Valid values 0 to 1.79769313486232E+308
  \[IsForegroundApp \<Boolean?\>\]: true if the user had active interaction with the app.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.devicemanagement/new-mgbetadevicemanagementuserexperienceanalyticbatteryhealthappimpact](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.devicemanagement/new-mgbetadevicemanagementuserexperienceanalyticbatteryhealthappimpact)



