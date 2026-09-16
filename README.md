# Anna Bonadimani — Portfolio

Sito portfolio personale di Anna Bonadimani, UX/UI Designer con background da ingegnere. Presenta i progetti selezionati, il percorso professionale e formativo, e le competenze tecniche.

## Struttura del progetto

- `index.html` — home page: hero e sezione "Selected Works"
- `about.html` — pagina About: Professional Experience, Education, Hard Skills
- `project-greentrips.html` — pagina di dettaglio progetto Green Trips (case study, in lavorazione)
- `project-supportapp.html` — pagina di dettaglio progetto IT Support Desktop App (case study, in lavorazione)
- `scss/` — sorgenti Sass, un partial per sezione (`_header`, `_hero`, `_works`, `_entries`, `_footer`, `_sections`, `_project-placeholder`, `_variables`, `_base`), importati da `style.scss`
- `css/style.css` — CSS compilato (con sourcemap), collegato da tutte le pagine HTML
- `assets/` — immagini, foto e icone del sito

## Stack tecnico

- HTML5 + Sass (Dart Sass)
- [Bootstrap 5](https://getbootstrap.com/) — solo grid system e utility (`bootstrap-grid.css`, `bootstrap-utilities.css`), via CDN, usato per i layout a colonne (Selected Works, sezioni About, form di contatto)
- [Google Fonts](https://fonts.google.com/) (Inter) e [Font Awesome](https://fontawesome.com/) per le icone social
- Form di contatto gestito da [FormSubmit](https://formsubmit.co/), nessun backend proprio

## Sviluppo

Il sito è statico: basta aprire i file HTML in un browser, oppure servirli con un server locale, ad esempio:

```bash
npx http-server
```

Le modifiche di stile vanno fatte nei file `.scss` dentro `scss/`, poi ricompilate in `css/style.css`:

```bash
npx sass scss/style.scss css/style.css --source-map
```
