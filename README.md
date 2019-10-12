# [hlidacstatu.github.io](https://hlidacstatu.github.io)

Tento repositář obsahuje zdrojové kódy pro [hlidacstatu.github.io](https://hlidacstatu.github.io/). Využíváme GitHub pages se šablonovacím systémem Jekyll.

## Přidání repozitáře
Repozitáře zobrazované na stránce, včetně zařazení do kategorií, jsou načítané z konfiguračního souboru [_config.yml](https://github.com/HlidacStatu/hlidacstatu.github.io/blob/master/_config.yml#L5). Přidání nového repozitáře tedy znamená jeho doplnění do tohoto souboru a vytvoření Pull requestu.

## Změna šablony
Pokud chcete upravit HTML šablonu, postupujte dle instrukcí v článku [Setting up your GitHub Pages site locally with Jekyll](https://help.github.com/articles/setting-up-your-github-pages-site-locally-with-jekyll/) (některé kroky není potřeba dělat pokud nevytváříte nový repozitář pro Github pages).

Jelikož aktuální šablona využívá [repository metadata](https://help.github.com/articles/repository-metadata-on-github-pages/) pro dynamické zobrazení některých informací o repozitáři (popis, počet forků, sledujících), budete také potřebovat nastavit token viz. článek [Using repository metadata locally](https://help.github.com/articles/repository-metadata-on-github-pages/#using-repository-metadata-locally).

Pak už jen stačí zavolat následující příkaz, který stránku přegeneruje při každém uložení:

```
JEKYLL_GITHUB_TOKEN=<yourtoken> bundle exec jekyll serve --verbose
```
