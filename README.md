# client-blueprint-vue3

Vue3, Vite og Typescript oppsetting for nye prosjekter på klient side

## Hva brukes repoet for?
Repoet brukes for å lage klient side generelt og er tilpasset for bruk internt i WP plugins.

## Kom i gang

```bash
# Installer alle pakker fra NPM (node_modules)
$ npm i

#  Build koden
$ npm run build

# Skal du jobbe med koden, da kan du watche endringer (OBS: fungerer ikke fra Vagrant. Kjør det gjerne fra maskina di): 
$ npm run watch
```


## Hvordan kan man bruke client-blueprint-vue3 i WP plugin
1. Klone repoet
```bash
$ git clone https://github.com/UKMNorge/client-blueprint-vue3 klient
```

2. Lage pekere til JS og CSS
```php
// I hovedfilen av WP plugin

wp_enqueue_style('UKMstatistikkVueStyle', plugin_dir_url(__FILE__) . '/klient/dist/assets/build.css');
wp_enqueue_script('UKMstatistikkVueJs', plugin_dir_url(__FILE__) . '/klient/dist/assets/build.js','','',true);
```
