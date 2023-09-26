<!-- Start SDK Example Usage -->


```go
package main

import(
	"context"
	"log"
	m7kgggopetstore "github.com/speakeasy-sdks/m7KGG-go-petstore"
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