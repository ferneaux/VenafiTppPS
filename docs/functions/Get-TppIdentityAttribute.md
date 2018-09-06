# Get-TppIdentityAttribute

## SYNOPSIS
Get attribute values for TPP objects

## SYNTAX

```
Get-TppIdentityAttribute [-PrefixedUniversalId] <String[]> [-Attribute] <String[]> [[-TppSession] <TppSession>]
 [<CommonParameters>]
```

## DESCRIPTION
Get attribute values for TPP identity objects

## EXAMPLES

### EXAMPLE 1
```
Get-TppIdentityAttribute -PrefixedUniversalId 'AD+mydomain.com:1234567890olikujyhtgrfedwsqa' -Attribute 'surname'
```

PrefixedUniversalId                              Attribute
-------------------                              ---------
AD+mydomain.com:1234567890olikujyhtgrfedwsqa {@{Name=surname; Value=Brownstein}}

Get Surname attribute for specific user

## PARAMETERS

### -PrefixedUniversalId
The id that represents the user or group. 
Use Get-TppIdentity to get the id.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: PrefixedUniversal

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Attribute
Retrieve identity attribute values for the users and groups. 
Attributes include Group Membership, Name, Internet Email Address, Given Name, Surname.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases:

Required: True
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TppSession
Session object created from New-TppSession method. 
The value defaults to the script session object $TppSession.

```yaml
Type: TppSession
Parameter Sets: (All)
Aliases:

Required: False
Position: 3
Default value: $Script:TppSession
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable.
For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### PrefixedUniversalId
## OUTPUTS

### PSCustomObject with the properties PrefixedUniversalId and Attribute
## NOTES

## RELATED LINKS

[http://venafitppps.readthedocs.io/en/latest/functions/Get-TppIdentityAttribute/](http://venafitppps.readthedocs.io/en/latest/functions/Get-TppIdentityAttribute/)

[https://github.com/gdbarron/VenafiTppPS/blob/master/VenafiTppPS/Public/Get-TppIdentityAttribute.ps1](https://github.com/gdbarron/VenafiTppPS/blob/master/VenafiTppPS/Public/Get-TppIdentityAttribute.ps1)

[https://docs.venafi.com/Docs/18.2SDK/TopNav/Content/SDK/WebSDK/API_Reference/r-SDK-POST-Identity-Readattribute.php?tocpath=REST%20API%20reference%7CIdentity%20programming%20interfaces%7C_____7](https://docs.venafi.com/Docs/18.2SDK/TopNav/Content/SDK/WebSDK/API_Reference/r-SDK-POST-Identity-Readattribute.php?tocpath=REST%20API%20reference%7CIdentity%20programming%20interfaces%7C_____7)
