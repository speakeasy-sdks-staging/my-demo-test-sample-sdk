<!-- Start SDK Example Usage -->


```go
package main

import (
	"context"
	mydemotestsamplesdk "github.com/speakeasy-sdks-staging/my-demo-test-sample-sdk"
	"log"
)

func main() {
	s := mydemotestsamplesdk.New()

	ctx := context.Background()
	res, err := s.Pets.CreatePets(ctx)
	if err != nil {
		log.Fatal(err)
	}

	if res.StatusCode == http.StatusOK {
		// handle response
	}
}

```
<!-- End SDK Example Usage -->