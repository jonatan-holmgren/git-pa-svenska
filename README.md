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
| pull        | pulla          | rycka         |
| push        | pusha          | knuffa        |
| fetch       | fetcha         | hämta         |
| branch      | brancha        | förgrena      |
| commit      | commita        | förbinda      |
| rebase      | rebasa         | ympa          |
| merge       | merga          | sammanfoga    |
| squash      | squasha        | mosa          |
| stash       | stasha         | gömma         |
| tag         | tagga          | märka         |
| cherry-pick | cherry-picka   | plocka russin |
| amend       | amenda         | rätta till    |
| blame       | blamea         | klandra       |

| Substantiv   | Nuvarande bruk | Förslag     |
|--------------|----------------|-------------|
| git          | git            | jävel       |
| repository   | repo           | förvaring   |
| branch       | branch         | gren        |
| commit       | commit         | förbindelse |
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
gitmiljö. Följande kommandon ändrar din `~/.gitconfig` och 
kommer att verka globalt.

    git config --global alias.ryck.command pull
    git config --global alias.knuffa.command push
    git config --global alias.gren.command branch
    git config --global alias.förgrena.command branch
    git config --global alias.förbind.command commit
    git config --global alias.ympa.command rebase
    git config --global alias.sammanfoga.command merge
    git config --global alias.göm.command stash
    git config --global alias.klandra.command blame
    git config --global alias.marke.command tag
    git config --global alias.mark.command tag

    alias jävel=git
