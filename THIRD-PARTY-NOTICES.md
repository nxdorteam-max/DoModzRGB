# Composants tiers et disponibilité des sources

Le code original de DoModz RGB est distinct des composants ci-dessous. Les licences tierces restent applicables, y compris leurs droits de modification et de remplacement. L’installateur ne contient pas le code original de DoModz RGB.

Les publications de https://github.com/nxdorteam-max/DoModzRGB/releases fournissent **ThirdParty-Sources-3.2.0.zip** à côté de l’installateur. Cette archive contient uniquement les sources et paquets des composants tiers ; elle ne contient pas le code original privé de DoModz RGB.

| Composant | Version / référence | Licence / source |
|---|---|---|
| OpenRGB, programme séparé | 8e16de2 / 1.1 | GPL-2.0 ; archive complète, instructions de compilation et dépendances incluses ; https://github.com/CalcProgrammer1/OpenRGB |
| Qt Base, Qt 5 Compat | 6.8.3 | LGPL-3.0 pour les bibliothèques distribuées ; sources complètes des modules et licences associées fournies |
| libusb | 1.0.27 | LGPL-2.1 ; sources fournies |
| hidapi-hotplug | 0.15.0 | Licence BSD fournie par HIDAPI ; sources de la variante hotplug fournies |
| PawnIO | 2.2.0 | GPL-2.0 ; source et sous-module PawnPP fournis ; pilote officiel redistribué sans modification |
| LibreHardwareMonitor | 0.9.6 | MPL-2.0 ; bibliothèque non modifiée et sources fournies |
| DiskInfoToolkit | 1.1.2, 25319eae | MPL-2.0 ; sources et paquet NuGet fournis |
| RAMSPDToolkit-NDD | 1.4.2, 3b47b960 | MPL-2.0 ; sources et paquet NuGet fournis |
| BlackSharp.Core | 1.0.7, c70b735c | MPL-2.0 ; sources et paquet NuGet fournis |
| HidSharp | 2.6.4 | Apache-2.0 ; notice et licence jointes |
| Bibliothèques .NET additionnelles | versions du manifeste de distribution | MIT ; notice Microsoft jointe |
| AMD ADLX SDK | commit indiqué dans ADLX-revision.txt | Licence AMD jointe ; le pilote AMD installé fournit l’implémentation ADLX |
| nlohmann/json | 3.12.0 | MIT ; notice jointe |
| Microsoft Visual C++ Runtime | redistribuable x64 officiel | Licence Microsoft du redistribuable ; installateur officiel signé conservé sans modification |
| DirectX Shader Compiler / DXIL | binaires de la distribution OpenRGB | Licences Microsoft / LLVM ; notices dans la source Qt/OpenRGB et notice DirectX jointe |

OpenRGB conserve son exécutable autonome et communique avec DoModz via son protocole SDK TCP local. Les bibliothèques LGPL ne sont ni incorporées au code original, ni chiffrées ou verrouillées contre leur remplacement. DoModz n’impose aucune interdiction d’analyse visant à déboguer des modifications de ces bibliothèques.

Les archives de sources comprennent leurs instructions de construction. Les archives Qt correspondent aux modules qtbase et qt5compat 6.8.3. Les DLL du moteur OpenRGB n’ont pas été modifiées. Les numéros de version, origines et empreintes des fichiers distribués figurent dans `DEPENDENCIES.json`.
