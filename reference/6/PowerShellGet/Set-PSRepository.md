---
ms.date:  2017-06-09
schema:  2.0.0
locale:  en-us
keywords:  powershell,cmdlet
online version:  http://go.microsoft.com/fwlink/?LinkId=821671
external help file:  PSModule-help.xml
title:  Set-PSRepository
---

# Set-PSRepository

## SYNOPSIS
Sets values for a registered repository.

## SYNTAX

```
Set-PSRepository -Name <String> [-SourceLocation <Uri>] [-PublishLocation <Uri>] [-ScriptSourceLocation <Uri>]
 [-ScriptPublishLocation <Uri>] [-Credential <PSCredential>] [-InstallationPolicy <String>] [-Proxy <Uri>]
 [-ProxyCredential <PSCredential>] [-PackageManagementProvider <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Set-PSRepository** cmdlet sets values for a registered module repository.

## EXAMPLES

### Example 1: Set the installation policy for a repository
```
PS C:\> Set-PSRepository -Name "myInternalSource" -InstallationPolicy Trusted
```

This command sets the installation policy for the myInternalSource repository to Trusted, so that users are not prompted before installing modules from that source.

### Example 2: Set the source and publish locations for a repository
```
PS C:\> Set-PSRepository -Name "myInternalSource" -SourceLocation 'http://someNuGetUrl.com/api/v2' -PublishLocation 'http://someNuGetUrl.com/api/v2/packages'
```

This command sets the source location and publish location for myInternalSource to the specified URIs.

## PARAMETERS

### -InstallationPolicy
Specifies the installation policy.
Valid values are: Trusted, UnTrusted.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 
Accepted values: Trusted, Untrusted

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Name
Specifies the name of the repository.

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

### -PackageManagementProvider
Specifies the package management provider.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PublishLocation
Specifies the URI of the publish location.
For example, for NuGet-based repositories, the publish location is similar to http://someNuGetUrl.com/api/v2/Packages.

```yaml
Type: Uri
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ScriptPublishLocation


```yaml
Type: Uri
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ScriptSourceLocation


```yaml
Type: Uri
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SourceLocation
Specifies the URI for discovering and installing modules from this repository.
For example, for NuGet-based repositories, the source location is similar to http://someNuGetUrl.com/api/v2.

```yaml
Type: Uri
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Credential


```yaml
Type: PSCredential
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Proxy


```yaml
Type: Uri
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ProxyCredential


```yaml
Type: PSCredential
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-PSRepository](Get-PSRepository.md)

[Register-PSRepository](Register-PSRepository.md)

[Unregister-PSRepository](Unregister-PSRepository.md)

