# TIG326 Övningar 
Repositoryt innehåller filer och exempel som används under git-workshopen i TIG326.

## Att göra 1
* klona det här repositoryt
* skapa en issue per föreläsning i kursen
* skapa en branch för den föreläsningstitel du vill lägga till
* lägg till en föreläsningstitel i filen lectures.md 
* commit, push, pull request (använd commit -m för att stänga issuen)


## Att göra 2
* Skapa ett eget repo
* initiera
* checka ut
* skapa en fil readme.md
* commit, push
* låt en kompis klona repot, branch, göra ändringa, och skicka ändringarna till din repo

## Att göra 3
* klona repot
* vad finns det för branches i repot?
* gör en ändring i en annan branch än main
* pull request

## Att göra 4
* Simulera en mergekonflikt:
  1. Två personer klonar samma repo.
  2. Båda skapar en branch och redigerar **samma rad** i `lectures.md`.
  3. Den ena gör pull request först – den andra får en konflikt.
  4. Lös konflikten lokalt (ni kan göra detta i VSCode istället):
     ```bash
     git pull origin main
     # redigera manuellt
     git add .
     git commit
     git push
     ```

## Att göra 5
* Utforska repo-historiken:
  1. Använd kommandon (ni kan göra detta i VSCode istället):
     ```bash
     git log
     git diff
     git blame lectures.md
     ```
  2. Ta reda på:
     - Vem har gjort senaste ändringen i `lectures.md`?
     - Hur många commits har du gjort?

## Att göra 6
* Använd GitHub Issues och koppla till commit:
  1. Skapa en issue: "Lägg till en föreläsningstitel"
  2. Skapa en branch, gör ändringen
  3. Commita med (ni kan göra detta i VSCode istället):
     ```bash
     git commit -m "Fixes #X Lägg till föreläsningstitel"
     ```
  4. Gör pull request → se att issuen stängs automatiskt

## Att göra 7
* Skapa en release:
  1. När `lectures.md` är klart, tagga versionen (ni kan göra detta i VSCode istället):
     ```bash
     git tag -a v1.0 -m "Första versionen klar"
     git push origin v1.0
     ```
  2. Gå till GitHub → fliken "Releases" → se versionen.
