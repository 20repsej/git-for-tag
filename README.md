# Git på svenska

## Introduktion

Det dagliga språket för de olika kommandona i `git` (eller `jävel`) är
på svenska ett enda stort svengelskakalas. Jag finner mig själv ofta
sägandes _"Kan du pusha branchen?"_ eller _"Jag pullar!"_, vilket
känns pinsamt.

Detta dokument ämnar etablera en ren svensk jargong som kan användas
på arbetsplatsen för att med fördel undvika pressade situationer med
kollegor samt boskap.

## Förslag

Nedan följer tabeller över verb och substantiv relaterade till git,
deras nuvarande bruk samt förslag på hur vi tillsammans kan bättra
oss.

| Verb        | Nuvarande bruk | Förslag       |
|-------------|----------------|---------------|
| pull        | pulla          | rycka         | dra, lok
| push        | pusha          | knuffa        | körtillstånd
| fetch       | fetcha         | hämta         |
| branch      | brancha        | förgrena      |
| commit      | commita        | förbinda      | påstigning
| rebase      | rebasa         | ympa          | rangera
| merge       | merga          | sammanfoga    | koppling
| squash      | squasha        | mosa          |
| stash       | stasha         | gömma         | urspårning
| tag         | tagga          | märka         | tåg
| cherry-pick | cherry-picka   | plocka russin |
| amend       | amenda         | rätta till    | rep
| blame       | blamea         | klandra       | signalfel, lövhalka, trafikverket, lokfel, banarbete

| Substantiv   | Nuvarande bruk | Förslag     |
|--------------|----------------|-------------|
| git          | git            | jävel       | klarerare
| repository   | repo           | förvaring   | bangård
| branch       | branch         | gren        | spår
| commit       | commit         | förbindelse | tågläge, koppla
| pull request | pull request   | ryckbegäran |
| stash        | stash          | gömma       |
| tag          | tagg           | märke       |

## Exempel

    - Kan du rycka grenen jag just ympade och knuffa till github?

    - Jag förgrenade alldeles nyss och förband ändringarna från min gömma där.

    - Skicka en ryckbegäran när du är färdig med sammanfogningen!

    - Låt oss plocka russin från mäster-grenen.
    
    - Hoppsan, jag råkade visst kraftknuffa mot mäster-grenen.. D:

    - Mosa dina förbindelser innan du sammanfogar.

## Dagligt bruk

Nedan följer en rad kommandoradskommandon för att sätta upp en svensk
gitmiljö. Avsaknaden av svenska tecken i täcknamnen beror på en brist i git
(överväg att förbättra mjukvaran och skicka en ryckbegäran!). Följande
kommandon ändrar din `~/.gitconfig` och kommer att verka globalt.

    git config --global alias.ryck pull
    git config --global alias.knuffa push
    git config --global alias.gren branch
    git config --global alias.forgrena branch
    git config --global alias.forbinda commit
    git config --global alias.ympa rebase
    git config --global alias.sammanfoga merge
    git config --global alias.gom stash
    git config --global alias.klandra blame
    git config --global alias.marke tag
    git config --global alias.mark tag

    alias jävel=git
