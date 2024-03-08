<!-- Start SDK Example Usage [usage] -->
```go
package main

import (
	"context"
	m7kgggopetstore "github.com/speakeasy-sdks/m7KGG-go-petstore"
	"github.com/speakeasy-sdks/m7KGG-go-petstore/pkg/models/shared"
	"log"
)

func main() {
	s := m7kgggopetstore.New()

	ctx := context.Background()
	res, err := s.Pets.CreatePets(ctx, shared.Pet{
		ID:   596804,
		Name: "<value>",
	})
	if err != nil {
		log.Fatal(err)
	}
	if res != nil {
		// handle response
	}
}

```
<!-- End SDK Example Usage [usage] -->