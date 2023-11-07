# AshTesting SDK


## Overview

Pokémon API: An API for retrieving Pokémon, Natures, and Stats

### Available Operations

* [GetNatureIDOrName](#getnatureidorname) - Retrieve a Nature by ID or name
* [GetPokemonIDOrName](#getpokemonidorname) - Retrieve a Pokémon by ID or name
* [GetStatIDOrName](#getstatidorname) - Retrieve a Stat by ID or name

## GetNatureIDOrName

Retrieve a Nature by ID or name

### Example Usage

```go
package main

import(
	"context"
	"log"
	testingplaygroundsdk "github.com/speakeasy-sdks/testing-playground-sdk"
	"github.com/speakeasy-sdks/testing-playground-sdk/pkg/models/operations"
)

func main() {
    s := testingplaygroundsdk.New()

    ctx := context.Background()
    res, err := s.GetNatureIDOrName(ctx, operations.GetNatureIDOrNameRequest{
        IDOrName: "string",
    })
    if err != nil {
        log.Fatal(err)
    }

    if res.StatusCode == http.StatusOK {
        // handle response
    }
}
```

### Parameters

| Parameter                                                                                  | Type                                                                                       | Required                                                                                   | Description                                                                                |
| ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ |
| `ctx`                                                                                      | [context.Context](https://pkg.go.dev/context#Context)                                      | :heavy_check_mark:                                                                         | The context to use for the request.                                                        |
| `request`                                                                                  | [operations.GetNatureIDOrNameRequest](../../models/operations/getnatureidornamerequest.md) | :heavy_check_mark:                                                                         | The request object to use for the request.                                                 |


### Response

**[*operations.GetNatureIDOrNameResponse](../../models/operations/getnatureidornameresponse.md), error**


## GetPokemonIDOrName

Retrieve a Pokémon by ID or name

### Example Usage

```go
package main

import(
	"context"
	"log"
	testingplaygroundsdk "github.com/speakeasy-sdks/testing-playground-sdk"
	"github.com/speakeasy-sdks/testing-playground-sdk/pkg/models/operations"
)

func main() {
    s := testingplaygroundsdk.New()

    ctx := context.Background()
    res, err := s.GetPokemonIDOrName(ctx, operations.GetPokemonIDOrNameRequest{
        IDOrName: "string",
    })
    if err != nil {
        log.Fatal(err)
    }

    if res.StatusCode == http.StatusOK {
        // handle response
    }
}
```

### Parameters

| Parameter                                                                                    | Type                                                                                         | Required                                                                                     | Description                                                                                  |
| -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- |
| `ctx`                                                                                        | [context.Context](https://pkg.go.dev/context#Context)                                        | :heavy_check_mark:                                                                           | The context to use for the request.                                                          |
| `request`                                                                                    | [operations.GetPokemonIDOrNameRequest](../../models/operations/getpokemonidornamerequest.md) | :heavy_check_mark:                                                                           | The request object to use for the request.                                                   |


### Response

**[*operations.GetPokemonIDOrNameResponse](../../models/operations/getpokemonidornameresponse.md), error**


## GetStatIDOrName

Retrieve a Stat by ID or name

### Example Usage

```go
package main

import(
	"context"
	"log"
	testingplaygroundsdk "github.com/speakeasy-sdks/testing-playground-sdk"
	"github.com/speakeasy-sdks/testing-playground-sdk/pkg/models/operations"
)

func main() {
    s := testingplaygroundsdk.New()

    ctx := context.Background()
    res, err := s.GetStatIDOrName(ctx, operations.GetStatIDOrNameRequest{
        IDOrName: "string",
    })
    if err != nil {
        log.Fatal(err)
    }

    if res.StatusCode == http.StatusOK {
        // handle response
    }
}
```

### Parameters

| Parameter                                                                              | Type                                                                                   | Required                                                                               | Description                                                                            |
| -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- |
| `ctx`                                                                                  | [context.Context](https://pkg.go.dev/context#Context)                                  | :heavy_check_mark:                                                                     | The context to use for the request.                                                    |
| `request`                                                                              | [operations.GetStatIDOrNameRequest](../../models/operations/getstatidornamerequest.md) | :heavy_check_mark:                                                                     | The request object to use for the request.                                             |


### Response

**[*operations.GetStatIDOrNameResponse](../../models/operations/getstatidornameresponse.md), error**

