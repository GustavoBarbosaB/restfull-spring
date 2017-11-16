# RestFull Service

***Este é um serviço RestFull que é capaz de fazer GET, POST, PUT e DELETE utilizando o Spring Framework 5.0.***

## Exemplo do JSON retornado na API:
```json
[
   {
        "id": 1,
        "name": "Saveiro",
        "cor": "Preta",
        "marca": "Volkswagen",
        "placa": "AAA-111"
    },
    {
        "id": 2,
        "name": "Gol",
        "cor": "Preta",
        "marca": "Volkswagen",
        "placa": "AAA-111"
    },
    {
        "id": 3,
        "name": "Golf",
        "cor": "Preta",
        "marca": "Volkswagen",
        "placa": "AAA-111"
    }
]
```

## Exemplo de JSON usado em um POST:
> O id é atribuido pela própria API
```json
{
        "name": "Golf",
        "cor": "Preta",
        "marca": "Volkswagen",
        "placa": "AAA-111"
}

```

## Exemplo de JSON usado em um PUT:
> Os campos passados serão alterados caso exista carro com id correspondente
> URL: http://localhost:8080/changeCar/1 
```json
{
        "name": "Golf",
        "cor": "Preta",
}

```

## URL's para GET e POST
***GET todos os carros***
> http://localhost:8080/car

***GET carro por marca***
>http://localhost:8080/car/{Marca}

***GET carro por marca e cor***
>http://localhost:8080/car/{Marca}?cor=Preta

***DELETE carro***
>http://localhost:8080/deleteCar/{idCar}

***PUT carro***
>http://localhost:8080/changeCar/{idCar}
