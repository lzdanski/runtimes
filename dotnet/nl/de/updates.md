---

copyright:
  years: 2015, 2017
lastupdated: "2017-10-06"
---

{:new_window: target="_blank"}
{:codeblock: .codeblock}

# Neueste Aktualisierungen für das Buildpack 'ASP.NET Core'
{: #latest_updates}


Eine Liste mit den neuesten Aktualisierungen im aspnet-Buildpack.

## 6. Oktober 2017: ASP.NET Core-Buildpack v1.0.26-20170913-1346 aktualisiert
* Unterstützung für .NET Core-Laufzeit 2.0.0 hinzugefügt
* Unterstützung für .NET Core SDK 1.1.0 hinzugefügt
* Unterstützung für .NET Core SDK 2.0.0 hinzugefügt
* Unterstützung für .NET Core SDK 1.1.0-preview1-005051 entfernt
* Unterstützung für .NET Core SDK 2.0.0-preview1-005977 entfernt
* Unterstützung für .NET Core-Laufzeit Version 1.0.3 entfernt
* Unterstützung für .NET Core-Laufzeit Version 1.1.0 entfernt
* Knotenversion auf 6.11.2 aktualisiert
* Standardversion von .NET Core SDK in 2.0.0 geändert
* Standardversion von .NET Core SDK für F#-Projekte in 1.1.0 geändert

## 24. Juli 2017: ASP.NET Core Buildpack v1.0.22-20170724-0813 aktualisiert

* Unterstützung für .NET Core-Laufzeit 2.0.0 Preview 2 hinzugefügt
* Unterstützung für .NET Core SDK 1.1.0-preview1-005051 hinzugefügt
* Unterstützung für .NET Core SDK 2.0.0-preview2-006497 hinzugefügt
* Knotenversion auf 6.11.1 aktualisiert
* Eigenständige Anwendungen stets ausführbar gemacht

## 20. Juni 2017: ASP.NET Core Buildpack v1.0.20-20170620-1449 aktualisiert

* Unterstützung für .NET Core-Laufzeit 2.0.0 Preview 1 hinzugefügt
* Unterstützung für .NET Core SDK 2.0.0-preview1-005977 hinzugefügt
* Knotenversion auf 6.10.3 aktualisiert
* Unterstützung für .NET Core-Laufzeit Version 1.0.0 entfernt
* Unterstützung für .NET Core-Laufzeit Version 1.0.1 entfernt
* Unterstützung für .NET Core SDK Version 1.0.0-preview2-1-003177 entfernt
* Datei 'staging_task.log' zu Anwendungscontainer hinzugefügt
* Geringere Plattenbelegung beim Caching von Abhängigkeiten

## 12. Mai 2017: ASP.NET Core Buildpack v1.0.18-20170516-1601 aktualisiert

* Unterstützung für .NET Core-Laufzeit 1.0.5 hinzugefügt
* Unterstützung für .NET Core-Laufzeit 1.1.2 hinzugefügt
* Unterstützung für .NET Core SDK 1.0.3 hinzugefügt
* Unterstützung für .NET Core SDK 1.0.4 hinzugefügt
* Knotenversion auf 6.10.2 aktualisiert
* Unterstützung für .NET Core SDK 1.0.1 entfernt
* Unterstützung für .NET Core SDK 1.0.0-preview4-004233 entfernt
* Verwendung der Umgebungsvariablen ASPNETCORE_URLS zum Angeben des Ports

## 29. März 2017: ASP.NET Core Buildpack v1.0.13-20170330-1023 aktualisiert

* Unterstützung für .NET Core-Laufzeit 1.0.4 hinzugefügt
* Unterstützung für .NET Core-Laufzeit 1.1.1 hinzugefügt
* Unterstützung für .NET Core SDK 1.0.1 hinzugefügt
* Knotenversion auf 6.10.0 aktualisiert
* Unterstützung für .NET Core SDK 1.0.0-preview2-003131 entfernt
* Unterstützung für .NET Core SDK 1.0.0-preview3-004056 entfernt

## 31. Januar 2017: ASP.NET Core-Buildpack v1.0.10-20170124-1145 aktualisiert

* Unterstützung für .NET Core 1.0.3 hinzugefügt
* Unterstützung für .NET Core MSBuild-Tool hinzugefügt
* Unterstützung für F#-Projekte hinzugefügt
* Unterstützung für .NET Core SDK 1.0.0-preview2-003121 entfernt

## 9. Dezember 2016: ASP.NET Core-Buildpack v1.0.6-20161205-0912 aktualisiert

* Unterstützung für .NET Core 1.1.0 hinzugefügt
* Unterstützung für .NET Core 1.0.0 RC2 entfernt
* Option zum Bereinigen des NuGet-Paketcaches hinzugefügt

## 10. Oktober 2016: Buildpack 'ASP.NET Core' v1.0.1-20161005-1225 aktualisiert.

* Unterstützung für .NET Core 1.0.1 hinzufügen
* Sporadisch auftretender Fehler, der beim Caching von NuGet-Packages zum Fehlschlagen der Bereitstellung führt

## 31. August 2016: Buildpack 'ASP.NET Core' v1.0-20160826-1345 aktualisiert.

* Unterstützung für die Ausführung von Prä- und Postkompilierscripts unter Verwendung von NPM und Bower hinzufügen, um Front-End-JavaScript- und CSS-Bibliotheken zu installieren.
* Buildpack von der Betaversion in den GA-Status versetzen

## 11. Juli 2016: Buildpack 'ASP.NET Core' v0.9-20160706-1603 aktualisiert

Diese Version des Buildpacks enthält die folgenden Änderungen:

* Diese Version des Buildpacks unterstützt .NET CLI 1.0 Preview 2 Build und .NET Core 1.0 RTM
* Das Buildpack unterstützt weiterhin .NET CLI 1.0 Preview 1 und .NET Core 1.0 RC2
* Die .NET CLI-Standardversion, die installiert wird, ist jetzt 1.0.0-preview2-003121

## 10. Juni 2016: Buildpack 'ASP.NET Core' v0.8.1-20160526-0957 aktualisiert

Diese Version des Buildpacks enthält die folgenden Änderungen:

* Der Name der Laufzeit wird von ASP.NET 5 in ASP.NET Core geändert.
* Die Buildpackversionsnummer ist in der Ausgabe des Erkennungsscripts enthalten.
* Diese Version des Buildpacks entfernt die Unterstützung von DNX-basierten Anwendungen, die CoreCLR RC1 und niedriger verwenden.
* Diese Version des Buildpacks unterstützt .NET CLI und .NET Core RC2.
* Das Buildpack erkennt Projekte mit einer Datei 'project.json' oder Dateien '*.runtimeconfig.json' in der Veröffentlichungsausgabe (publish).

## 22. Oktober 2015: Buildpack 'ASP.NET 5' v0.7-20151022-1257 aktualisiert

* Diese Version des Buildpacks entfernt Mono und unterstützt dafür die Beta-8-CoreCLR.

## 18. September 2015: Buildpack 'ASP.NET 5' v0.6-20150916-1220 aktualisiert

* Diese Version des Buildpacks unterstützt Beta-7-DNX-Änderungen und kann mithilfe des folgenden angepassten Startbefehls Anwendungen ausführen, die von älteren Betaversionen abhängig sind:

```
   dnx src/dotnetstarter kestrel --server.urls http://${VCAP_APP_HOST}:${PORT}
```
{: codeblock}

* Die Verwendung des Nowin-Web-Servers wurde in diesem Buildpack entfernt. Dafür wird der [Kestrel]{https://github.com/aspnet/KestrelHttpServer}-Web-Server verwendet.

# Zugehörige Links
{: #rellinks notoc}
## Allgemein
{: #general notoc}
* [Dotnet Core-Laufzeit](index.html)
