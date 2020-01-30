
```javascript
// Welcome!
let languages = {
    english: 'Welcome',
    czech: 'Vitejte',
    danish: 'Velkomst',
    dutch: 'Welkom',
    estonian: 'Tere tulemast',
    finnish: 'Tervetuloa',
    flemish: 'Welgekomen',
    french: 'Bienvenue',
    german: 'Willkommen',
    irish: 'Failte',
    italian: 'Benvenuto',
    latvian: 'Gaidits',
    lithuanian: 'Laukiamas',
    polish: 'Witamy',
    spanish: 'Bienvenido',
    swedish: 'Valkommen',
    welsh: 'Croeso'
}
function greet(language) {
    for(let k in languages){
        if(k == language){
            return languages[k];
        }
    }
    return "Welcome";
}

//Duck Duck Goose
function duckDuckGoose(players, goose) {
  while (players.length < goose) {
    goose = goose - players.length
  }
  return players[goose - 1].name
}
```