# quotesapi
### quotes-from-all-over-the-world API
#### This api is created with Ruby on rails using postgresql. To understand this api, follow the instructions

[Lets go to Quote-api](https://quotes-from-all-over-the-world.herokuapp.com/api/v1/quotes)

## API Documentation
### Suported languages: en
### Public routes
GET /quotes (get all quotes) params: [page, per, search]
GET /quotes/2 (get quote show by id)
GET /quotes/random (get random quote)  by default it shows one quote but use can use params: [nb] for limit of quotes





## GET /quotes
![A test image](quote-api.png)

### thats how it look like the index of quotes

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
    ]
  }
```
## we can use you Get /quotes with three parameters
#### /qoutes?page
#### /qoutes?per
#### /qoutes?search
