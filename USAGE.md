<!-- Start SDK Example Usage -->
```go
package main

import (
	"context"
	m7kgggopetstore "github.com/speakeasy-sdks/m7KGG-go-petstore"
	"log"
	"net/http"
)

func main() {
	s := m7kgggopetstore.New()

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