- Add Linux support
- Add New-TppDevice
- New-TppCapiApplication
    - Add ProvisionCertificate parameter to provision a certificate when the application is created
    - Removed UpdateIis switch as unnecessary, simply use WebSiteName
    - Add ApplicationName parameter to support pipelining of path
    - Add SkipExistenceCheck parameter to bypass some validation which some users might not have access to

- New-TppCertificate
    - Certificate authority is no longer required
    - Fix failure when SAN parameter not provided
    - Fix Management Type not applying
- Add ability to provide root level path, \ved, in some `Find-` functions
- Add pipelining and ShouldProcess functionality to multiple functions
- Update New-TppObject to make Attribute not mandatory
- Remove ability to write to the log with built-in event groups.  This is no longer supported by Venafi.  Custom event groups are still supported.
- Add aliases for Find-TppObject (fto), Find-TppCertificate (ftc), and Invoke-TppCertificateRenewal (itcr)
