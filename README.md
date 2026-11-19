# TL187 Private AI Platform: releases

Signed Windows installers and the update feed (`latest.yml`) that installed copies of
**TL187 Private AI Platform** read to update themselves. The source repository is private;
this repository holds release assets only.

Every installer, app executable, uninstaller and elevation helper is Authenticode-signed by
**TECHLEAD 187 LLC** (Azure Artifact Signing, RFC 3161 timestamp). The app refuses an update
that is not signed by that publisher.

Verify a download in PowerShell:

```powershell
Get-AuthenticodeSignature '.\TL187 Private AI Platform Setup <version>.exe' | Format-List Status, SignerCertificate
```

Compare its SHA-256 with the value in the release notes.

Tech Lead 187 LLC · https://techlead187.com
