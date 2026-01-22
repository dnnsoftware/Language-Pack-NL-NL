# Suggesties voor verbeterde Nederlandse vertalingen

Dit document bevat suggesties voor het verbeteren van de Nederlandse vertalingen in dit taalpack voor DNN (DotNetNuke). De suggesties zijn gebaseerd op een analyse van de bestaande vertalingen en de richtlijnen in [COMMON_TERMS.md](.github/COMMON_TERMS.md).

## 📋 Samenvatting

Er zijn **163 vertaalbestanden** (.resx) geanalyseerd. Over het algemeen is de kwaliteit van de vertalingen goed, maar er zijn een aantal consistentie- en stijlproblemen gevonden die kunnen worden verbeterd.

## 🔍 Gevonden problemen en suggesties

### 1. Inconsistente spelling van "creëren/creeëren"

**Probleem**: Er worden verschillende spellingen gebruikt voor het woord "creëren".

**Voorbeelden van huidige inconsistenties**:
- `creeëren` (foutief - dubbele 'e' en trema)
- `creëren` (correct - enkele 'e' en trema)

**Gevonden locaties**:
- `Resources/App_GlobalResources/Exceptions.nl-NL.resx` (regel 94): "Fout bij het creeëren van de BusinessControllerClass"
- `Resources/App_GlobalResources/Exceptions.nl-NL.resx` (regel 100): "oneindige omleidingslus creeërt"
- `Resources/DesktopModules/Admin/Dnn.PersonaBar/Modules/Dnn.Pages/App_LocalResources/pages.nl-NL.resx`: "hiërarchie te creeëren"
- `Resources/DesktopModules/SocialGroups/App_LocalResources/SharedResources.nl-NL.resx`: "het creëren van een landingspagina"

**Aanbeveling**: 
- Gebruik consistent **"creëren"** (met één 'e' en trema) in alle vertalingen
- Vervang alle voorkomsten van "creeëren" door "creëren"
- Overweeg alternatieven zoals "aanmaken", "maken" of "toevoegen" waar dat natuurlijker klinkt

### 2. Gebruik van formele "U/Uw" vorm in plaats van informele "je/jouw"

**Probleem**: De richtlijnen specificeren het gebruik van de informele "jij/je" vorm, maar op diverse plaatsen wordt nog de formele "U/Uw" vorm gebruikt.

**Gevonden locaties**:
- `Resources/admin/Modules/App_LocalResources/ModuleSettings.ascx.nl-NL.resx`: "U kunt de kalender popup gebruiken" (2 voorkomsten)
- `Resources/DesktopModules/Admin/Dnn.PersonaBar/Modules/Dnn.TaskScheduler/App_LocalResources/taskscheduler.nl-NL.resx`: "Uw wijzigingen zijn opgeslagen"
- `Resources/DesktopModules/Admin/Dnn.PersonaBar/Modules/Dnn.Users/App_LocalResources/users.nl-NL.resx`: "Uw configuratie vereist" (2 voorkomsten)
- `Resources/DesktopModules/Admin/Dnn.PersonaBar/Modules/Dnn.Pages/App_LocalResources/pages.nl-NL.resx`: "Uw site heeft geen thema's"
- `Resources/DesktopModules/Admin/Dnn.PersonaBar/Modules/Dnn.Recyclebin/App_LocalResources/recyclebin.nl-NL.resx`: "U kunt eenvoudig" (2 voorkomsten)
- `Resources/DesktopModules/Admin/Dnn.PersonaBar/Modules/Dnn.SiteImportExport/App_LocalResources/SiteImportExport.nl-NL.resx`: "Uw data export" (2 voorkomsten)
- `Resources/DesktopModules/Admin/Dnn.PersonaBar/Modules/Dnn.SiteSettings/App_LocalResources/sitesettings.nl-NL.resx`: meerdere voorkomsten
- `Resources/DesktopModules/Admin/Dnn.PersonaBar/Modules/Dnn.ConfigConsole/App_LocalResources/configconsole.nl-NL.resx`: "Uw configuratie bestand"
- `Resources/DesktopModules/Admin/Dnn.PersonaBar/Modules/Dnn.Licensing/App_LocalResources/licensing.nl-NL.resx`: "Uw licensie" (meerdere voorkomsten)

**Aanbeveling**:
- Vervang alle voorkomsten van "U" door "je" of "jij"
- Vervang alle voorkomsten van "Uw" door "je" of "jouw"
- Let op: soms zal "je" voldoende zijn, bijvoorbeeld: "U kunt" → "Je kunt" of "Je kan"

### 3. Inconsistent gebruik van "portaal" vs. "site"

**Probleem**: Volgens COMMON_TERMS.md moet "portal" vertaald worden als "site", maar "portaal" wordt nog op veel plaatsen gebruikt.

**Gevonden voorbeelden**:
- `Resources/App_GlobalResources/Exceptions.nl-NL.resx`: "Het portaal heeft geen ruimte ter beschikking" (2 voorkomsten)
- `Resources/App_GlobalResources/Exceptions.nl-NL.resx` (regel 94): "portaal ({4})"
- `Resources/App_GlobalResources/Prompt.nl-NL.resx`: meerdere voorkomsten van "portaal"

**Aanbeveling**:
- Vervang "portaal" door "site" waar het verwijst naar de DNN portal/website
- Behoud "portaal" alleen als het een technische term is in een specifieke context waar wijzigen verwarrend zou zijn
- Volgens de terminologiegids: portal settings = siteinstellingen, niet portaalinstellingen

### 4. Inconsistent gebruik van "tab" in technische context

**Probleem**: "Tab" wordt in de code en berichten gebruikt, maar zou volgens de richtlijnen "pagina" moeten zijn.

**Gevonden voorbeelden**:
- `Resources/App_GlobalResources/Exceptions.nl-NL.resx` (regel 94): "tab ({3})"
- Diverse locaties waar "tab" wordt gebruikt in technische berichten

**Aanbeveling**:
- Overweeg "tab" te vervangen door "pagina" waar het verwijst naar pagina's in DNN
- Let op: in sommige contexten (zoals UI tabs) kan "tab" of "tabblad" passend zijn
- Voeg eventueel een toelichting toe dat intern "tab" en "page" door elkaar worden gebruikt

### 5. Hoofdlettergebruik in labels

**Probleem**: Volgens de richtlijnen moet alleen het eerste woord een hoofdletter hebben, maar dit wordt niet altijd consequent toegepast.

**Voorbeeld**:
- `Resources/App_GlobalResources/GlobalResources.nl-NL.resx`: "Neem Contact met ons op" moet zijn "Neem contact met ons op"

**Aanbeveling**:
- Controleer alle labels en pas het hoofdlettergebruik aan volgens de richtlijn
- Alleen het eerste woord krijgt een hoofdletter (tenzij het een eigennaam is)

### 6. Inconsistente aanhalingstekens en interpunctie

**Probleem**: In foutmeldingen worden verschillende soorten aanhalingstekens gebruikt.

**Voorbeelden**:
- Enkelvoudige aanhalingstekens: `'{0}'`
- Dubbele aanhalingstekens: `"{0}"`

**Aanbeveling**:
- Kies voor consistente aanhalingstekens (bij voorkeur enkele aanhalingstekens voor technische termen)
- Zorg voor consistente interpunctie aan het einde van zinnen (wel of geen punt)

### 7. Anglicismen en leenwoorden

**Probleem**: Sommige Engelse termen worden direct overgenomen terwijl er goede Nederlandse alternatieven zijn.

**Voorbeelden**:
- "Invoice" in licensing berichten → "factuur"
- "Sales Dept." → "verkoopafdeling"

**Aanbeveling**:
- Vervang Engelse termen door Nederlandse equivalenten waar mogelijk
- Behoud alleen technische Engelse termen waar geen goed Nederlands alternatief bestaat

### 8. Samentrekking en spatiegebruik bij samenstellingen

**Probleem**: Volgens de richtlijnen moeten woorden in de Nederlandse vorm aan elkaar geschreven worden.

**Observatie**: 
- Over het algemeen wordt dit goed toegepast
- Sporadisch zouden er nog verbeteringen kunnen zijn

**Aanbeveling**:
- Controleer samenstellingen zoals "profiel eigenschappen" → "profieleigenschappen"
- Zorg dat samengestelde woorden zonder spatie worden geschreven

## 📊 Prioritering

### Hoge prioriteit (consistentie en richtlijnen)
1. ✅ Vervangen van "U/Uw" door "je/jouw" (ca. 15-20 bestanden)
2. ✅ Corrigeren van "creeëren" naar "creëren" (ca. 5 bestanden)
3. ✅ Hoofdlettergebruik in labels (ca. 10-20 bestanden)

### Gemiddelde prioriteit (terminologie)
4. 📝 Vervangen van "portaal" door "site" waar van toepassing (ca. 20 bestanden)
5. 📝 Vervangen van Engelse termen door Nederlandse equivalenten (ca. 10 bestanden)

### Lage prioriteit (fijnafstemming)
6. 📝 Consistente aanhalingstekens en interpunctie
7. 📝 Gebruik van "tab" vs "pagina" in technische contexten

## 🎯 Aanbevolen werkwijze

1. **Start met één categorie per keer** - Begin met de hoge prioriteit items
2. **Maak aparte pull requests** - Groepeer wijzigingen logisch (bijv. alle "U/Uw" correcties samen)
3. **Test de wijzigingen** - Als mogelijk, test in een lokale DNN omgeving
4. **Documenteer de wijzigingen** - Verwijs naar dit document in de pull request beschrijvingen
5. **Vraag review** - Laat wijzigingen door minstens 2 personen beoordelen (zoals aangegeven in readme.md)

## 📝 Specifieke bestandssuggesties

### Bestand: `Resources/App_GlobalResources/Exceptions.nl-NL.resx`

**Regel 94**:
```xml
<!-- Huidig -->
<value>Fout bij het creeëren van de BusinessControllerClass '{0}' van module ({1}) id=({2}) in tab ({3}) en portaal ({4})</value>

<!-- Voorgesteld -->
<value>Fout bij het creëren van de BusinessControllerClass '{0}' van module ({1}) id=({2}) op pagina ({3}) en site ({4})</value>
```

**Regel 100**:
```xml
<!-- Huidig -->
<value>Het is niet mogelijk om een veld aan te maken met naam {0} omdat dit een oneindige omleidingslus creeërt.</value>

<!-- Voorgesteld -->
<value>Het is niet mogelijk om een veld aan te maken met naam {0} omdat dit een oneindige omleidingslus creëert.</value>
```

### Bestand: `Resources/App_GlobalResources/GlobalResources.nl-NL.resx`

**Regel 40**:
```xml
<!-- Huidig -->
<value>Neem Contact met ons op</value>

<!-- Voorgesteld -->
<value>Neem contact met ons op</value>
```

### Bestand: `Resources/admin/Modules/App_LocalResources/ModuleSettings.ascx.nl-NL.resx`

```xml
<!-- Huidig -->
<value>Voer een einddatum in voor weergave van deze module. Na deze datum wordt de module automatisch verborgen. U kunt de kalender popup gebruiken om een datum te selecteren.</value>

<!-- Voorgesteld -->
<value>Voer een einddatum in voor weergave van deze module. Na deze datum wordt de module automatisch verborgen. Je kunt de kalenderpopup gebruiken om een datum te selecteren.</value>
```

## 🔄 Volgende stappen

1. **Review dit document** - Bespreek deze suggesties met het vertaalteam
2. **Prioriteer de wijzigingen** - Bepaal welke wijzigingen als eerste doorgevoerd moeten worden
3. **Verdeel het werk** - Wijs verschillende categorieën toe aan verschillende bijdragers
4. **Maak pull requests** - Implementeer de wijzigingen volgens de aanbevolen werkwijze
5. **Update de richtlijnen** - Voeg eventueel extra voorbeelden toe aan COMMON_TERMS.md

## 📚 Bronnen

- [Taaladvies - Trema](https://taaladvies.net/taal/advies/vraag/1563/trema_in_creeren_en_reageren/)
- [Taalunie - Samenstellingen](https://taaladvies.net/samenstellingen/)
- [ANS - Nederlands woordenboek](https://ans.ivdnt.org/)

---

**Laatst bijgewerkt**: 2026-01-22  
**Versie**: 1.0  
**Auteur**: GitHub Copilot Coding Agent
