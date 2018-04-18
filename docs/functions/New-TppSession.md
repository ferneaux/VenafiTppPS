# New-TppSession

## SYNOPSIS
Create a new Venafi TPP session

## SYNTAX

### Credential
```
New-TppSession -ServerUrl <String> -Credential <PSCredential> [-PassThru] [<CommonParameters>]
```

### UsernamePassword
```
New-TppSession -ServerUrl <String> -Username <String> -SecurePassword <SecureString> [-PassThru]
 [<CommonParameters>]
```

## DESCRIPTION
Authenticates a user via a username and password against a configured Trust
Protection Platform identity provider (e.g.
Active Directory, LDAP, or Local).
After
the user is authenticated, Trust Protection Platform returns an API key allowing
access to all other REST calls.

## EXAMPLES

### EXAMPLE 1
```

```

## PARAMETERS

### -ServerUrl
URL for the Venafi server.

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

### -Credential
PSCredential object utilizing the same credentials as used for the web front-end

```yaml
Type: PSCredential
Parameter Sets: Credential
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Username
Username to authenticate to ServerUrl with

```yaml
Type: String
Parameter Sets: UsernamePassword
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SecurePassword
SecureString password to authenticate to ServerUrl with

```yaml
Type: SecureString
Parameter Sets: UsernamePassword
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PassThru
Optionally, send the session object to the pipeline.

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable.
For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

### PSCustomObject

## NOTES

## RELATED LINKS