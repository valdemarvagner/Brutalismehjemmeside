# AGENTS.md --- Studenternes Kunstforening Sjælland

## Projekt

Dette repository indeholder hjemmesiden til den fiktive forening
**Studenternes Kunstforening Sjælland (SKS)**.

Hjemmesiden udvikles som et skoleprojekt på multimediedesign. Den
visuelle hovedretning er **brutalisme / brutalist web design**, men
designet skal stadig være brugervenligt, responsivt og tilgængeligt.

Overordnet idé:

> Hvor kunst og fællesskab mødes i konstant udvikling.

Foreningen henvender sig primært til nuværende og tidligere studerende
med interesse for kunst og kultur.

------------------------------------------------------------------------

## Arbejdsprincip

Når du hjælper med kode eller foreslår ændringer, skal du prioritere i
denne rækkefølge:

1.  Semantisk HTML
2.  Brugervenlighed
3.  Tilgængelighed
4.  Responsivt design
5.  Overskuelig og genbrugelig CSS
6.  Overensstemmelse med Figma-designet
7.  Den brutalistiske visuelle identitet
8.  Enkel teknisk implementering

Undgå at gøre løsningen mere kompleks end nødvendigt.

------------------------------------------------------------------------

## Teknologi

Projektet skal primært bygges med:

-   HTML5
-   CSS3
-   Git

Bootstrap må kun bruges, hvis det er et bevidst valg og ikke overtager
hjemmesidens visuelle identitet.

Brug ikke JavaScript, frameworks eller eksterne biblioteker, medmindre
de er nødvendige eller specifikt efterspurgt.

Brug ikke Canva i projektet.

------------------------------------------------------------------------

## HTML

HTML skal være semantisk og kunne valideres.

Foretræk relevante HTML-elementer som:

-   `header`
-   `nav`
-   `main`
-   `section`
-   `article`
-   `figure`
-   `footer`
-   `form`
-   `label`
-   `button`

Brug ikke `div` som erstatning for et mere passende semantisk element.

Der skal kun være én primær `h1` pr. side. Overskriftsniveauer skal
følge en logisk struktur.

Links bruges til navigation. Buttons bruges til handlinger.

Billeder skal have meningsfulde `alt`-tekster, medmindre de er rent
dekorative.

Formularfelter skal have korrekte labels. Brug native HTML-controls, fx
`input type="radio"`, når de findes.

------------------------------------------------------------------------

## CSS

CSS skal være let at læse og vedligeholde.

Foretræk:

-   CSS custom properties til farver, spacing, borders og andre
    design-tokens
-   Flexbox til endimensionelle layouts
-   CSS Grid til større grids og sidekompositioner
-   Mobile-first responsive CSS
-   Genbrugelige klasser frem for gentagelse
-   Få, tydelige breakpoints

Eksempel på struktur:

``` css
:root {
  --color-background: #fff;
  --color-text: #000;
  --border-width: 2px;

  --space-xs: 0.5rem;
  --space-sm: 1rem;
  --space-md: 2rem;
  --space-lg: 4rem;
}
```

Undgå:

-   Unødvendig `!important`
-   Store mængder inline CSS
-   Tilfældige pixelværdier uden forbindelse til designsystemet
-   Overdrevet nesting eller meget specifikke selectors
-   Unødvendige animationer

------------------------------------------------------------------------

## Brutalistisk designretning

Designet skal tydeligt kunne forbindes med brutalistisk webdesign.

Arbejd blandt andet med:

-   Markant typografi
-   Store overskrifter
-   Høj kontrast
-   Synlige borders
-   Tydelige grids
-   Asymmetri, når det har et formål
-   Rektangulære UI-elementer
-   Rå sort/hvide/rasteriserede billeder
-   Direkte visuel kommunikation
-   Nummerering og funktionelle labels som `[01]`, `[02]`
-   Begrænset eller markant farvepalette

Brutalisme betyder **ikke** automatisk kaos eller dårlig usability.

Eksperimenterende elementer må ikke gøre navigation, formularer eller
vigtig information svær at forstå.

Undgå som standard:

-   Store border-radius-værdier
-   Bløde shadows
-   Glassmorphism
-   Gradienter uden en klar designmæssig begrundelse
-   Generiske moderne SaaS-cards
-   Dekoration uden funktion

------------------------------------------------------------------------

## Typografi

Typografien skal have et tydeligt hierarki.

Den aktuelle retning kan arbejde med:

-   Tung grotesk/display-font til store overskrifter
-   Neutral grotesk til brødtekst
-   Monospace til metadata, datoer, labels og eventnumre

Mulige fonte, hvis de vælges i designet:

-   Archivo / Archivo Black
-   Space Grotesk
-   IBM Plex Mono

Introducer ikke nye fonte uden grund. Hold helst designsystemet til
højst to fontfamilier.

Typografien skal fortsat være læsbar på små skærme.

------------------------------------------------------------------------

## Billedstil

Projektet arbejder med en rå brutalistisk billedstil.

Mulige virkemidler:

-   Sort/hvid
-   Høj kontrast
-   Raster/halftone
-   Tætte beskæringer
-   Rå Photoshop-behandling
-   Editoriale billedkompositioner

Mindst ét billede eller grafisk element skal være bearbejdet i
Photoshop.

Brug ikke kraftig billedbehandling på alle billeder, hvis det gør
kunstværker eller vigtig information svære at aflæse.

------------------------------------------------------------------------

## Layout og Gestalt

Designbeslutninger skal kunne begrundes med relevante designprincipper.

Vær især opmærksom på:

-   Visuelt hierarki
-   Kontrast
-   Alignment
-   Repetition
-   Balance
-   Proximity
-   Similarity
-   Common region
-   Figure/ground
-   Continuity

Eksempel: Gentagne eventkort med samme border, typografi og struktur kan
bruge **similarity** og **repetition**, mens deres borders skaber
**common region**.

Gestaltprincipper skal bruges funktionelt og ikke kun nævnes som teori.

------------------------------------------------------------------------

## Responsive design

Hjemmesiden skal fungere på både mobil og desktop.

Ved mindre skærme:

-   Lad grids gå fra flere kolonner til én eller færre kolonner
-   Reducér store display-overskrifter
-   Bevar tydeligt informationshierarki
-   Sørg for tilstrækkelige touch targets
-   Undgå horisontal scrolling, medmindre det er en bevidst og nødvendig
    funktion
-   Sørg for at billeder skalerer korrekt

Brutalistiske desktop-kompositioner må gerne forenkles på mobil.

------------------------------------------------------------------------

## Tilgængelighed

Visuel eksperimentering må ikke ske på bekostning af accessibility.

Sørg for:

-   God farvekontrast
-   Synlige focus states
-   Keyboard-navigation
-   Korrekte labels på formularer
-   Meningsfulde linktekster
-   Alt-tekster
-   Logisk heading-struktur
-   Tilstrækkeligt store klikområder
-   At information ikke kommunikeres gennem farve alene

Fjern ikke browserens focus outline uden at erstatte den med en tydelig
focus state.

------------------------------------------------------------------------

## Sider og indhold

Projektet kan blandt andet indeholde:

### Forside

Skal hurtigt kommunikere SKS, kommende aktiviteter og en tydelig vej
videre.

### Events / udstillinger

Kan præsentere kunstudstillinger, workshops, foredrag og andre
aktiviteter.

En udstillingsside må gerne være meget billedbåret og bruge et
asymmetrisk editorialt grid.

### Om os

Skal forklare foreningen, dens formål, aktiviteter og fællesskab.

### Bliv medlem

Skal først forklare værdien af medlemskab og derefter gøre indmeldelsen
enkel.

Formularen skal prioritere usability. Hvis brugeren skal vælge mellem fx
"Studerende" og "Tidligere studerende", bruges radio buttons.

------------------------------------------------------------------------

## Content

Opfind ikke faktuelle oplysninger om SKS, som ikke findes i
projektmaterialet.

Det gælder eksempelvis:

-   Medlemspriser
-   Adresser
-   Eventdatoer
-   Kunstnernavne
-   Antal medlemmer
-   Dokumenterede målgruppepræferencer

Brug tydelige placeholders, hvis oplysninger mangler.

Eksempel:

``` text
XX KR. / ÅR
[DATO]
[STED]
[KUNSTNERNAVN]
```

Designhypoteser må ikke fremstilles som brugerresearch.

------------------------------------------------------------------------

## Målgruppe

Den foreløbige målgruppe arbejder med unge voksne omkring 18--30 år,
især nuværende og tidligere studerende med interesse for kunst og
kultur.

Mere specifikke antagelser om fx:

-   Visuelle præferencer
-   Street-kultur
-   Brutalisme
-   Retrofuturisme
-   Sociale medier
-   Motivation for museumsbesøg

skal behandles som hypoteser, indtil de understøttes af research.

Designet skal udvikles på baggrund af faktisk research frem for at
opfinde brugerbehov.

------------------------------------------------------------------------

## Figma

Figma er designets source of truth for wireframes og mock-ups.

Ved implementering:

-   Følg Figma-layoutets hierarki
-   Genbrug spacing og størrelser systematisk
-   Oversæt Figma-grids til passende CSS Grid/Flexbox
-   Undgå at hardcode positioner alene for at efterligne et screenshot
-   Implementér designet responsivt frem for kun at ramme én viewport

Hvis kode og Figma er i konflikt, skal forskellen identificeres i stedet
for at gætte på intentionen.

------------------------------------------------------------------------

## Komponenter

Genbrug mønstre for blandt andet:

-   Navigation
-   Buttons
-   Eventkort
-   Billedmoduler
-   Labels
-   Formularfelter
-   CTA-sektioner
-   Footer

Komponenterne skal visuelt hænge sammen gennem samme typografi,
border-system, spacing og interaktionsprincipper.

------------------------------------------------------------------------

## Filstruktur

Hold strukturen enkel og forståelig. Et eksempel:

``` text
/
├── index.html
├── events.html
├── om-os.html
├── bliv-medlem.html
├── css/
│   └── style.css
├── images/
│   ├── events/
│   └── graphics/
└── README.md
```

Tilpas strukturen til det faktiske projekt. Opret ikke filer eller
mapper, som ikke er nødvendige.

------------------------------------------------------------------------

## Når du ændrer kode

Når du hjælper med projektet:

1.  Undersøg eksisterende struktur og styles først.
2.  Genbrug eksisterende design-tokens og komponenter.
3.  Lav den mindst omfattende ændring, der løser problemet korrekt.
4.  Bevar semantisk HTML og accessibility.
5.  Kontrollér responsive konsekvenser.
6.  Undgå at omskrive fungerende kode uden grund.
7.  Forklar større strukturelle ændringer kort.

Hvis information mangler, spørg eller brug en tydelig placeholder i
stedet for at opfinde detaljer.

------------------------------------------------------------------------

## Kvalitetskontrol

Før en større ændring betragtes som færdig, kontrollér så vidt muligt:

-   HTML-validering
-   CSS-validering
-   Mobilvisning
-   Desktopvisning
-   Keyboard-navigation
-   Focus states
-   Billeders `alt`-tekster
-   Formularlabels
-   Heading-hierarki
-   Links og navigation
-   At der ikke er utilsigtet horizontal overflow
-   At implementeringen stadig følger Figma og den brutalistiske
    designretning

------------------------------------------------------------------------

## Projektets vigtigste regel

Alle større valg skal så vidt muligt kunne forbindes:

**Målgruppe → research → brutalistisk stil → designvalg → Figma →
HTML/CSS → færdigt website.**

Prioritér et sammenhængende og begrundet design frem for at tilføje
brutalistiske effekter tilfældigt.

