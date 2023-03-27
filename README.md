# v-13.2-exercises
# Övning - Movie search app

## Instruktioner

Du ska bygga en sida där man kan söka på filmer och visa resultatet i en lista. Ifall sökningen inte ger några träffar ska ett meddelande om detta visas.

Du ska använda dig av nedanstående API för att göra sökningen.

**API:** http://www.omdbapi.com/

**API-nyckel:** 37fe945a

Exempelanrop:

```
fetch('http://www.omdbapi.com/?apikey=37fe945a&s=Emma');
```

`s=Emma` är själva sökordet. Alltså `s=` säger vad man ska söka på i API:et och därefter kan man mata in en filmtitel.

Du ska visa följande egenskaper om varje film:
* imdbID
* Poster
* Title
* Year

## Tekniska krav
Din React-app ska bestå (förutom index.js och app.jsx) av tre komponenter:

 * `SearchMovies.jsx` - För att söka mot API:et
 * `DisplayMovies.jsx` - Ska loopa ut alla filmer som sökningen returnerade, varje film ska vara komponenten `MovieCard`
 * `MovieCard.jsx` - En komponent för att visa en film med ovanstående egenskaper

Använd dig av funktionella komponenter, `useState` och props.
