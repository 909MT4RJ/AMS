# A.M.S. – updates

Deze repository bevat **alleen de installers** van A.M.S. (Automotive
Management System) voor Autobedrijf Coen Droomers, als downloads onder
**Releases**. De broncode staat hier niet.

A.M.S. kijkt zelf (bij het opstarten en daarna elke 4 uur) naar de nieuwste
release hier, downloadt die op de achtergrond en toont een knop
**"Update x.y.z staat klaar – Nu installeren"**.

## Hoe een nieuwe versie hier komt

Een nieuwe versie wordt als commit op de branch `upload` gezet (de installer
`AMS-Setup-x.y.z.exe`, de `.blockmap` en `latest.yml`). De workflow
`.github/workflows/release.yml` maakt daar automatisch de release `vx.y.z`
van. De branch `upload` wordt elke keer vervangen, zodat de repository klein
blijft; de installers staan alleen bij de releases.

**Deze repository moet openbaar blijven**, anders kan A.M.S. de updates niet
ophalen. Er staan geen gegevens van klanten of wachtwoorden in.
