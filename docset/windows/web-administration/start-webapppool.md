---
author: brianlic-msft
description: 
external help file: Microsoft.IIS.PowerShell.Provider.dll-Help.xml
keywords: powershell, cmdlet
manager: alanth
ms.date: 2016-12-27
ms.prod: powershell
ms.technology: powershell
ms.topic: reference
online version: 
schema: 2.0.0
title: Start-WebAppPool
ms.assetid: EA40251C-40A4-4AA8-B7D7-728775713F9E
---

# Start-WebAppPool

## SYNOPSIS
Starts an application pool.

## SYNTAX

```
Start-WebAppPool [[-Name] <String>] [-Passthru] [<CommonParameters>]
```

## DESCRIPTION
The **Start-WebAppPool** cmdlet starts the specified application pool.

## EXAMPLES

### Example 1: Start an application pool
```
IIS:\> Start-WebAppPool -Name "DefaultAppPool"
```

This command starts the application pool named DefaultAppPool.

### Example 2: Start stopped application pools
```
IIS:\> Get-ChildItem IIS:\AppPools | where {$_.state -eq "Started"} | Start-WebAppPool
```

This command starts the application pools that are currently stopped.

## PARAMETERS

### -Name
Specifies the name of the application pool to start.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Passthru
Passes an object that represents the application pool to the pipeline.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[New-WebAppPool](./New-WebAppPool.md)

[Remove-WebAppPool](./Remove-WebAppPool.md)

[Restart-WebAppPool](./Restart-WebAppPool.md)

[Stop-WebAppPool](./Stop-WebAppPool.md)
