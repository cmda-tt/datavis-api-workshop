![Guide Banner](https://raw.githubusercontent.com/cmda-tt/datavis-api-workshop/main/images/guide-banner.svg)

# Getting started

👋 In deze workshop gaan we werken met [Python](https://www.python.org/) in [Jupyter Notebooks](https://jupyter.org/) stijl. Over het algemeen beschouwd als 'de standaard' toolcombinatie in data science en information design.

Python is een programmeertaal die bekend staat om gemakkelijk leesbaar en schrijfbaar te zijn waardoor het goed en snel te leren is. Daarnaast is Python een goede keuze omdat er veel libraries beschikbaar zijn specifiek voor data-analyse waardoor je code niet 'from scratch' hoeft te schrijven maar ingebouwde functies van de libraries kunt gebruiken.

Jupyter is een stuk software om 'notebooks' te maken. Het is een populair hulpmiddel bovenop Python omdat je code, documentatie en output in 1 overzichtelijk formaat hebt. Je maakt 'interactieve code' in de vorm van cellen waarbij je heel stapsgewijs kunt werken en ondertussen het resultaat van je code kunt zien en documenteren wat de code doet.

We gaan drie dingen installeren:

1. Python als programmeertaal installeren
2. Jupyter als notebook formaat installeren
3. VSCode en extensions instellen

Laten we aan de slag gaan om deze tools op je computer te zetten!

## 1. Python installeren

We gebruiken de huidige standaard release van Python om notebooks te runnen. Alles boven versie `+3.8` is prima. Je kunt Python installeren via de installer (voor de meeste mensen) van hun website of via de terminal (voor de nerds). Uiteindelijk voeren we een check uit om te kijken of de installatie is gelukt. Voor Jupyter is helaas geen installer, iedereen zal die via de Terminal moeten installeren (zie instructies).

### Python installeren via de installer

Via https://www.python.org/downloads/ kun je de python versie downloaden voor het operating system wat je hebt (Windows of MacOS). Open de installer en doorloop de stappen zoals je elk ander programma op je computer zou installeren.

#### Controle installatie

Je kunt checken of de installatie is gelukt door bijvoorbeeld in spotlight op Python te zoeken of via de Finder in je applications folder te kijken. Als het goed is zou er een applicatie genaamd 'Python Launcher' of 'IDLE' moeten zijn.

### Python installeren via de terminal (MacOS only)

**Voor MacOS:** Open de terminal door via spotlight te zoeken naar 'terminal' of via je finder in 'applications' > 'hulpprogramma's (utilities)

### **Installeer Homebrew**

Homebrew is een pakketbeheerder voor macOS waarmee je eenvoudig software kunt installeren. Kopieer het volgende commando in je terminal:

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

### **Installeer Python met Homebrew**

Als Homebrew is geïnstalleerd, kun je Python installeren door:

```bash
brew install python
```

Dit installeert de nieuwste versie van Python 3.

#### Controle installatie

Door `python3 --version` als commando uit te voeren krijg je als het goed is in de terminal het versienummer van je huidige python installatie terug.

## 2. Jupyter installeren

In beide gevallen installeer je Jupyter Notebook via pip in de terminal, er is helaas geen installer voor het installeren van Jupyter op je computer.

- **Voor MacOS:** Open de terminal door via spotlight te zoeken naar 'terminal' of via je finder in 'applications' > 'hulpprogramma's (utilities)'.
- **Voor Windows:** Open je zoekbalk en zoek naar 'command prompt' of 'powershell'.

Kopieer en plak het volgende commando en druk op `enter`.

```bash
pip install jupyter
```

## 3. VSCode installeren

Er zijn heel veel verschillende manieren om Jupyter Notebooks te runnen. Bijvoorbeeld via hun website of eigen Jupyterlabs applicatie maar wij raden aan om dat via VSCode te doen, zo kan je straks bij het eindproject goed samenwerken met de tech-trackers omdat zij dezelfde tools gebruiken.

### Code editor installeren

Om notebooks te draaien heb je een code editor nodig, we raden Visual Studio Code (VSCode) van Microsoft aan. Als je die niet op je computer hebt, installeer deze dan.

Ga naar de website van Visual Studio Code om de versie te downloaden voor je operating system:
[VSCode Downloads](https://code.visualstudio.com/Download). Na installatie open de code editor.

### Extensions installeren

Binnen VSCode downloaden we eental 'extensions' om te kunnen werken met Python syntax en om Jupyter notebooks te kunnen runnen.

2. **Installeer de Python-extensie**:

   - Open VS Code.
   - Ga naar de extensiemarkt door te klikken op het vierkante icoon aan de linkerkant (of gebruik `Ctrl+Shift+X`).
   - Zoek naar "Python" en installeer de extensie van Microsoft.

3. **Installeer de Jupyter-extensie**:
   - Ga opnieuw naar de extensiemarkt.
   - Zoek naar "Jupyter" en installeer de extensie van Microsoft.

### Virtual Env maken

Om een aantal packages als libraries in een notebook te kunnen runnen moet je een virtual environemnt aanmaken.

1. **Maak een map aan op je computer**

   - Maak via je finder of windows verkenner een map aan op je computer bijvoorbeeld 'datavis-workshop'

2. **Plaats daarin een Jupyter Notebook**

    - Download de 'test-notebook.ipynb' bestand van deze GitHub repo.
    - Zet dit .ipynb bestand in de folder die je in de vorige stap hebt aangemaakt.

1. **Open de gemaakte map in je code editor**:

   - Ga naar `File` > `Open Folder...` en selecteer de map die je hebt aangemaakt ('e.g. datavis-workshop')

2. **Selecteer je 'kernel' om Notebooks mee te runnen.**

   - Klik op 'Select Kernel' rechtsbovenin als het goed is krijg je een dropdown. 
   - Klik op 'Select Another Kernel' als optie
   - Klik op 'Python Environments' als optie
   - Klik op 'Create Python Environment' als optie
   - Klik op 'Venv' als optie

   Als het goed is heb je nu een virtual environment aangemaakt. Je zou in je map een folder die `.venv` heet moeten zien.

### Notebook test runnen

3. **Run je notebook!**

- Klik bovenin op 'run all' om alle cells in de notebook in z'n geheel te runnen.
- Je kunt ook op het 'play icoontje' drukken bij individuele cellen om ze afzonderlijk van elkaar te runnen.

That's it! Als de output van de cellen zichtbaar zijn ben je klaar om met Jupyter Notebooks te werken in VS Code.
