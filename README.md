# Saludos en Go

Este paquete proporciona una forma simple de obtener saluodos personalizados en Go.

## Instalación

Ejecuta el siguiente comando para instalar el paquete:

```bash
go get -u github.com/domouling/greetings
```

## Uso

Aqui tienes un ejemplo de como utilizar el paquete en tu codigo:

```go
package main

import (
    "fmt"
    "github.com/domouling/greetings"
)

func main() {
    message, err := greetings.Hello("Gilberto")

    if err != nil {
        fmt.Println("Ocurrio un error: ", err)
    }

    fmt.Println(message)
}
```

Este ejemplo importa el paquete github.com/domouling/greetings y llama a la función Hello con un
saludo personalizado. Si ocurre un error, se imprime un mensaje de error.
