# Git-and-Github-LinkAcademy-2025-2026

Comenzi principale



1. Initializarea unui proiect git
# git init        //  Acesta se executa o singura data




2. Adaugarea unui fisier in staged 
# git add nume_fisier        // adaugam un singur fisier sau toate cu "."
 
3. Creare unui commit 
# git commit -m " .... mesajul propriu zis ...  "


Exista posibilitatea sa combin add si commit -> functioneaza doar pentru fisierele TRACKED
# git commit -am " .... mesajul propriu zis ...  "


4. Sincronizarea cu serverul
# git push



Comenzi vizualizare 

5. Pentru a vedea toate commit-urile
# git log 
Pentru a vedea sub forma de graph commiturile
# git log --graph 
Pentru a vedea sub forma de rezumat commiturile (un commit o singura linie)
# git log --oneline
Putem combina acesti parametri (flag)
# git log --graph --oneline

6. Pentru a vedea starea fisierelor
# git status
Pentru a vedea un status scurt
# git status -s
# git status --short


Comenzi de schimbare a unui commit 

Head^1 -> sterge 1 commit de la HEAD in jos
Soft -> fisierele din commit raman in STAGED (verde)
# git reset --soft HEAD^1 
MIXED -> fisierele din commit raman in MODIFIED (rosu)
# git reset --mixed HEAD^1 
HARD -> fisierele din commit sunt sterse -> atentie
# git reset --hard HEAD^1 