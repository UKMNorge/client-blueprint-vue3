# client-blueprint-vue3

Vue3, Vite og Typescript oppsetting for nye prosjekter på klient side

## Hva brukes repoet for?
Repoet brukes for å lage klient side generelt og er tilpasset for bruk internt i WP plugins.

## Kom i gang
- Installer alle pakker fra NPM (node_modules): 
``
npm i
``
- Build koden: 
``
npm run build
``
- Skal du jobbe med koden, da kan du watch endringer (OBS: fungerer ikke fra Vagrant. Kjør det gjerne fra maskina di): 
``
npm run watch
``


## Hvordan kan man bruke client-blueprint-vue3 i WP plugin
1. Klone dette repoet i hovedmape i plugin
2. Endre navn av **mappe client-blueprint-vue3** til **klient**
3. Lage pekere til JS og CSS (se Eksempel: pekere til JS og CSS fra WP plugin)


#### Eksempel: pekere til JS og CSS fra WP plugin
I hovedfilen av WP plugin, legg til: </br>
``
wp_enqueue_style('UKMstatistikkVueStyle', plugin_dir_url(__FILE__) . '/klient/dist/assets/build.css');
wp_enqueue_script('UKMstatistikkVueJs', plugin_dir_url(__FILE__) . '/klient/dist/assets/build.js','','',true);
``
