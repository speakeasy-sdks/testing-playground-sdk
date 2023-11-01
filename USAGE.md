<!-- Start SDK Example Usage -->


```go
package main

import (
	"context"
	testingplaygroundsdk "github.com/speakeasy-sdks/testing-playground-sdk"
	"github.com/speakeasy-sdks/testing-playground-sdk/pkg/models/operations"
	"log"
)

func main() {
	s := testingplaygroundsdk.New()

	ctx := context.Background()
	res, err := s.AshTesting.GetNatureIDOrName(ctx, operations.GetNatureIDOrNameRequest{
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
<!-- End SDK Example Usage -->