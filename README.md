# Bad Guy Quotes API (Forked from [Ron Swanson API](https://github.com/jamesseanwright/ron-swanson-quotes))

Because I was bored at work today 


## Production host

[Not Promising to keep this running](https://bad-guy-quotes.herokuapp.com/)

The `Access-Control-Allow-Origin` header is set to `*` so that you can make requests from any domain.

## APIs

### `GET /v2/quotes`

Returns an array with one quote:

```json
[
    "Capitalism: God’s way of determining who is smart and who is poor."
]
```

### `GET /v2/quotes/<count>`

Returns an array with `<count>` quotes e.g. `GET /quotes/2`

```json
[
    "Capitalism: God’s way of determining who is smart and who is poor.",
    "Clear alcohols are for rich women on diets."
]
```

## OpenAPI 3 Schema

An [OpenAPI](https://swagger.io/docs/specification/about/) 3 schema is available at `/v2/schema`. Thanks to [Chris Gali](https://github.com/chrisgali01) for the suggestion and the initial draft.

## JavaScript demo

[JSFiddle](http://jsfiddle.net/7g2w4dhc/27/) (requires a browser with support for `Promise`s, ES6, `fetch`, and generator functions.)

## Hubot integration

I wrote a Hubot script that can be installed via npm. See the [repo](https://github.com/jamesseanwright/hubot-swanson) for more details.
