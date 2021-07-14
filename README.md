# quotes api
### quotes-from-all-over-the-world API
This api is created with Ruby on rails using postgresql. we bring you over 59,000 world famous quotes with authors and their genre completely free.

## where is this API used
this API used in [Quote-guessing-game](https://quote-guessing-game.herokuapp.com/game)

_____________________

[Lets go to Quote-api](https://quotes-from-all-over-the-world.herokuapp.com/api/v1/quotes)

## API Documentation

Suported languages: english

### Public routes

GET [`/api/v1/quotes`](https://quotes-from-all-over-the-world.herokuapp.com/api/v1/quotes) (get all quotes)
 - With params we can use /quotes?page=2, /quotes?per=3
 - we can use search by name of author or quote like /quotes?search=life

GET [`/api/v1/quotes/2`](https://quotes-from-all-over-the-world.herokuapp.com/api/v1/quotes/2) (get quote show by id))

GET [`/api/v1/quotes/random`](https://quotes-from-all-over-the-world.herokuapp.com/api/v1/quotes/random) (get random quote))
  - By default it shows one quote. With params we can use /quotes/random?nb=2 for limiting quotes

GET [`/api/v1/authors`](https://quotes-from-all-over-the-world.herokuapp.com/api/v1/authors) (get all authors)
 - With params we can use /quotes?page=2, /quotes?per=3
 - we can use search by name of author like /quotes?search=life

GET [`/api/v1/authors/1`](https://quotes-from-all-over-the-world.herokuapp.com/api/v1/authors/1) (get author show by id)

GET [`/api/v1/authors/random`](https://quotes-from-all-over-the-world.herokuapp.com/api/v1/authors/random) (get random authors))
  - By default it shows two authors. With params we can use /authors/random?nb=2 for limiting quotes
  - you can use reject_id params for the author which you don't want to get in random list like /authors/random?reject_id=31


## GET /api/v1/quotes photo

![A test image](quote-api.png)

### thats how GET /api/v1/quotes look like

```sh
  { "quotes":
    [
      {
        "id":24483,
        "quote_text":"006 was such an interesting character and the film really explored his friendship with Bond and how it all went wrong, so it was a very personal journey for both characters.",
        "quote_author":"Sean Bean",
        "quote_genre":"friendship",
        "author_id":7617
      }
    ],
    "meta":
      {
        "page":0,
        "per":30,
        "nb_pages":1976,
        "search":null
      }
  }
```
### thats how GET /api/v1/quotes/1 look like

```sh
  {
    "id":1,
    "quote_text":"All diseases run into one, old age.","quote_author":"Ralph Waldo Emerson",
    "quote_genre":"age",
    "author_id":1
  }
```

### thats how GET /api/v1/quotes/1 look like

```sh
  {
    "random_quote":
      [
        {
          "id":3243,
          "quote_text":"Light in Nature creates the movement of colors.",
          "quote_author":"Robert Delaunay",
          "quote_genre":"art",
          "author_id":922
        }
      ]
  }
```
### thats how GET /api/v1/authors look like

```sh
  [
    {"id":1175,"name":"Aaliyah"},
    {"id":3300,"name":"A. A. Milne"},
    {"id":8886,"name":"Aaron Allston"},
    {"id":7160,"name":"Aaron Carter"}
  ]
```

### thats how GET /api/v1/authors/1 look like

```sh
  {
    "id":1,
    "name":"Ralph Waldo Emerson"
  }
```
### thats how GET /api/v1/authors/random look like

```sh
  {
    "random_authors":
      [
        {"id":5788,"name":"Luigi Pirandello"},
        {"id":8341,"name":"Melinda Clarke"}
      ]
  }
```
