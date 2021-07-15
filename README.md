# quotes api
### quotes-from-all-over-the-world API
This api is created with Ruby on rails using postgresql. we bring you over 59,000 world famous quotes with authors and their genre completely free.
To understand this api, check the instructions

[Lets go to Quote-api](https://quotes-from-all-over-the-world.herokuapp.com/api/v1/quotes)

## API Documentation

Suported languages: en

### Public routes

GET [`/api/v1/quotes`](https://quotes-from-all-over-the-world.herokuapp.com/api/v1/quotes) (get all quotes)
 - With params we can use /quotes?page=2, /quotes?per=3
 - we can use search by name of author and quotes like /quotes?search=life

GET [`/api/v1/quotes/2`](https://quotes-from-all-over-the-world.herokuapp.com/api/v1/quotes/2) (get quote show by id))

GET [`/api/v1/quotes/random`](https://quotes-from-all-over-the-world.herokuapp.com/api/v1/quotes/random) (get random quote))
  - By default it shows one quote. With params we can use /quotes/random?nb=2 for limiting quotes

GET [`/api/v1/authors`](https://quotes-from-all-over-the-world.herokuapp.com/api/v1/authors) (get all authors)
 - With params we can use /quotes?page=2, /quotes?per=3
 - we can use search by name of author like /quotes?search=life

GET [`/api/v1/authors/1`](https://quotes-from-all-over-the-world.herokuapp.com/api/v1/authors/1) (get author show by id)

GET [`/api/v1/authors/random`](https://quotes-from-all-over-the-world.herokuapp.com/api/v1/authors/random) (get random authors))
  - By default it shows two author. With params we can use /authors/random?nb=2 for limiting quotes
  - we can use reject id of author which you don't want to get in random like /authors/random?reject_id=31


## GET /api/v1/quotes photo

![A test image](quote-api.png)

### thats how it look like the GET /api/v1/quotes

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
