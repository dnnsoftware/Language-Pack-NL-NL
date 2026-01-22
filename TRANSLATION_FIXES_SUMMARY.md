# Samenvatting Nederlandse Vertaling Verbeteringen

## 📊 Uitgevoerde Wijzigingen

Dit document geeft een overzicht van de uitgevoerde verbeteringen aan de Nederlandse vertalingen in dit DNN taalpack.

### Datum: 2026-01-22

## ✅ Geïmplementeerde Wijzigingen

### 1. Spelling Correcties - "creeëren" → "creëren"

**Aantal wijzigingen: 3**

| Bestand | Regel | Oud | Nieuw |
|---------|-------|-----|-------|
| `Exceptions.nl-NL.resx` | 94 | "creeëren" | "creëren" |
| `Exceptions.nl-NL.resx` | 100 | "creeërt" | "creëert" |
| `pages.nl-NL.resx` | 94 | "creeëren" | "creëren" |

**Reden**: De correcte spelling in het Nederlands is "creëren" (met één 'e' en trema), niet "creeëren" (met dubbele 'e').

### 2. Formele/Informele Aanspreekvorm - "U/Uw" → "je/jouw"

**Aantal wijzigingen: 24 voorkomsten in 7 bestanden**

Volgens de [richtlijnen](.github/COMMON_TERMS.md) moet de informele "jij/je" vorm worden gebruikt in plaats van de formele "U/Uw" vorm.

#### Bestand: `ModuleSettings.ascx.nl-NL.resx` (9 wijzigingen)
- "als u deze module wilt" → "als je deze module wilt"
- "U kunt de kalender popup gebruiken" → "Je kunt de kalenderpopup gebruiken"
- "indien u dit leeg laat" → "indien je dit leeg laat"

#### Bestand: `taskscheduler.nl-NL.resx` (1 wijziging)
- "Uw wijzigingen zijn opgeslagen" → "Je wijzigingen zijn opgeslagen"

#### Bestand: `users.nl-NL.resx` (2 wijzigingen)
- "Uw configuratie vereist" → "Je configuratie vereist"
- "Uw nieuwe wachtwoord" → "Je nieuwe wachtwoord"

#### Bestand: `pages.nl-NL.resx` (1 wijziging)
- "Uw site heeft geen thema's" → "Je site heeft geen thema's"

#### Bestand: `SiteImportExport.nl-NL.resx` (2 wijzigingen)
- "Uw data export" → "Je data export"
- "Uw data import" → "Je data import"

#### Bestand: `configconsole.nl-NL.resx` (1 wijziging)
- "Uw configuratie bestand" → "Je configuratiebestand"

#### Bestand: `licensing.nl-NL.resx` (7 wijzigingen)
- "Uw licensie" → "Je licentie" (meerdere voorkomsten)
- "Uw verlengde proef licensie" → "Je verlengde proeflicentie"
- "Uw proeflicensieverlengingsverzoek" → "Je proeflicentieverlengingsverzoek"

### 3. Hoofdlettergebruik Correcties

**Aantal wijzigingen: 1**

| Bestand | Oud | Nieuw |
|---------|-----|-------|
| `GlobalResources.nl-NL.resx` | "Neem Contact met ons op" | "Neem contact met ons op" |

**Reden**: Volgens de richtlijnen moet alleen het eerste woord een hoofdletter hebben, tenzij het een eigennaam is.

### 4. Terminologie Verbeteringen

#### a. "portaal" → "site"
**Aantal wijzigingen: 2**
- "in tab ({3}) en portaal ({4})" → "op pagina ({3}) en site ({4})"

#### b. "Portaal beheerders" → "sitebeheerders"
**Aantal wijzigingen: 1**
- Consistent met de terminologiegids

#### c. "licensie" → "licentie"
**Aantal wijzigingen: 7**
- Correcte Nederlandse spelling gebruikt

#### d. "invoice" → "factuur"
**Aantal wijzigingen: 3**
- Nederlandse term gebruikt in plaats van Engels leenwoord

#### e. "Technisch Support" → "technische ondersteuning"
**Aantal wijzigingen: 3**
- Nederlandse term gebruikt

#### f. "Sales Dept." → "verkoopafdeling"
**Aantal wijzigingen: 1**
- Nederlandse term gebruikt

### 5. Samenstellingen Verbeterd

**Aantal wijzigingen: 2**
- "configuratie bestand" → "configuratiebestand"
- "kalender popup" → "kalenderpopup"

**Reden**: Volgens de richtlijnen moeten Nederlandse samenstellingen zonder spatie worden geschreven.

## 📈 Statistieken

- **Totaal aantal gewijzigde bestanden**: 10
- **Totaal aantal wijzigingen**: ~40 individuele vertalingen verbeterd
- **Belangrijkste categorieën**: 
  - Spelling: 3 wijzigingen
  - Formaliteit: 24 wijzigingen
  - Terminologie: 13+ wijzigingen

## 🔍 Resterende Aandachtspunten

### Potentiële Toekomstige Verbeteringen

1. **Resterende "U" vormen**: Er zijn nog enkele (3) voorkomsten van "U" in de bestanden die mogelijk aandacht behoeven, afhankelijk van de context.

2. **"portaal" vs "site"**: Er zijn nog meerdere voorkomens van "portaal" in de codebase. Deze moeten per geval worden beoordeeld:
   - In technische contexten (variabelnamen, log berichten) kan "portaal" behouden blijven
   - In gebruikersgerichte teksten moet "site" worden gebruikt

3. **"tab" vs "pagina"**: In sommige technische contexten wordt "tab" nog gebruikt waar "pagina" passender zou zijn volgens de richtlijnen.

4. **Interpunctie consistentie**: Aanhalingstekens en punt-gebruik aan het einde van foutmeldingen zou verder gestandaardiseerd kunnen worden.

## 📝 Aanbevelingen voor Bijdragers

### Voor Pull Requests
1. **Refereer naar TRANSLATION_IMPROVEMENTS.md** - Dit document bevat gedetailleerde suggesties voor verdere verbeteringen
2. **Volg de COMMON_TERMS.md richtlijnen** - Zorg voor consistente terminologie
3. **Test indien mogelijk** - Test wijzigingen in een lokale DNN omgeving
4. **Groepeer logisch** - Groepeer gerelateerde wijzigingen in één PR

### Kwaliteitscontrole Checklist
Bij het reviewen van Nederlandse vertalingen:
- [ ] Gebruik van informele "je/jouw" vorm (niet "U/Uw")
- [ ] Correcte spelling (bijv. "creëren" niet "creeëren")
- [ ] Hoofdlettergebruik: alleen eerste woord van labels
- [ ] Nederlandse samenstellingen zonder spaties
- [ ] Consistente terminologie volgens COMMON_TERMS.md
- [ ] Nederlandse alternatieven voor Engelse termen waar mogelijk

## 📚 Referenties

1. [TRANSLATION_IMPROVEMENTS.md](./TRANSLATION_IMPROVEMENTS.md) - Gedetailleerde suggesties voor verdere verbeteringen
2. [COMMON_TERMS.md](.github/COMMON_TERMS.md) - Officiële terminologie richtlijnen
3. [README.md](./readme.md) - Contributie richtlijnen

## 🎯 Impact

Deze wijzigingen verbeteren:
- **Consistentie** - Eenduidige aanspreekvorm en terminologie
- **Correctheid** - Spelling en grammatica verbeterd
- **Leesbaarheid** - Natuurlijker Nederlands
- **Professionaliteit** - Consequent taalgebruik

---

**Bijgewerkt**: 2026-01-22  
**Commit ID's**: 6b1ee8d, acdf4d9  
**Status**: ✅ Geïmplementeerd en gecommit
