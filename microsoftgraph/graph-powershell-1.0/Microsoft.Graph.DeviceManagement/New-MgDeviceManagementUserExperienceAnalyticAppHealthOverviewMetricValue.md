---
external help file: Microsoft.Graph.DeviceManagement-help.xml
Module Name: Microsoft.Graph.DeviceManagement
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.devicemanagement/new-mgdevicemanagementuserexperienceanalyticapphealthoverviewmetricvalue
schema: 2.0.0
---

# New-MgDeviceManagementUserExperienceAnalyticAppHealthOverviewMetricValue

## SYNOPSIS
Create new navigation property to metricValues for deviceManagement

> [!NOTE]
> To view the beta release of this cmdlet, view [New-MgBetaDeviceManagementUserExperienceAnalyticAppHealthOverviewMetricValue](/powershell/module/Microsoft.Graph.Beta.DeviceManagement/New-MgBetaDeviceManagementUserExperienceAnalyticAppHealthOverviewMetricValue?view=graph-powershell-beta)

## SYNTAX

### CreateExpanded (Default)
```
New-MgDeviceManagementUserExperienceAnalyticAppHealthOverviewMetricValue [-AdditionalProperties <Hashtable>]
 [-Id <String>] [-Unit <String>] [-Value <Double>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgDeviceManagementUserExperienceAnalyticAppHealthOverviewMetricValue
 -BodyParameter <IMicrosoftGraphUserExperienceAnalyticsMetric> [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create new navigation property to metricValues for deviceManagement

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
The user experience analytics metric contains the score and units of a metric of a user experience anlaytics category.
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphUserExperienceAnalyticsMetric
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

### -Unit
The unit of the user experience analytics metric.
Examples: none, percentage, count, seconds, score.

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

### -Value
The value of the user experience analytics metric.

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

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphUserExperienceAnalyticsMetric
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphUserExperienceAnalyticsMetric
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER \<IMicrosoftGraphUserExperienceAnalyticsMetric\>: The user experience analytics metric contains the score and units of a metric of a user experience anlaytics category.
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
  \[Unit \<String\>\]: The unit of the user experience analytics metric.
Examples: none, percentage, count, seconds, score.
  \[Value \<Double?\>\]: The value of the user experience analytics metric.

## RELATED LINKS
[New-MgBetaDeviceManagementUserExperienceAnalyticAppHealthOverviewMetricValue](/powershell/module/Microsoft.Graph.Beta.DeviceManagement/New-MgBetaDeviceManagementUserExperienceAnalyticAppHealthOverviewMetricValue?view=graph-powershell-beta)

[https://learn.microsoft.com/powershell/module/microsoft.graph.devicemanagement/new-mgdevicemanagementuserexperienceanalyticapphealthoverviewmetricvalue](https://learn.microsoft.com/powershell/module/microsoft.graph.devicemanagement/new-mgdevicemanagementuserexperienceanalyticapphealthoverviewmetricvalue)



