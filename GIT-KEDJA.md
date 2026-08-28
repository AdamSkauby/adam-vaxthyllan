## Ladda upp skelettfilerna till GitHub

Repo-adress:

```text
https://github.com/AdamSkauby/adam-vaxthyllan.git
```

Kör kommandona i denna ordning:

```bash
git status
git add index.html README.md
git commit -m "Skapa skelettfiler för webbplatsen - Adam och Bertil"
git remote add origin https://github.com/AdamSkauby/adam-vaxthyllan.git
git push -u origin HEAD
```

`git status` kontrollerar repots aktuella status och visar vilka filer som är ändrade.

`git add index.html README.md` väljer skelettfilerna som ska ingå i commiten.

`git commit` sparar filerna lokalt med ett tydligt meddelande som anger att Adam och Bertil har skapat skelettfilerna.

`git remote add origin` kopplar det lokala repot till GitHub-repot.

Om `origin` redan finns, som i detta repo, ska kommandot hoppas över. För att ändra adressen används i stället:

```bash
git remote set-url origin https://github.com/AdamSkauby/adam-vaxthyllan.git
```

`git push -u origin HEAD` laddar upp den aktuella commiten till GitHub och kopplar den aktuella lokala referensen till remote-repot. Ingen ny branch eller `git checkout` används.
