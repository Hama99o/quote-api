# quotesapi
### quotes-from-all-over-the-world API
#### This api is created with Ruby on rails using postgresql. To understand this api, follow the instructions

[Lets go to Quote-api](https://quotes-from-all-over-the-world.herokuapp.com/api/v1/quotes)

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
### we can use you Get /quotes with three parameters
## /qoutes?page
## /qoutes?per
## /qoutes?search
