# API specification


## Models
### User
```ts
    {
        username: string;
        password: string;
        id: number;
    }
```

## Users
### POST /login
#### Request
```ts
    {
        username: string;
        password: string;
    }
```

#### Response
```ts
    {
        response: "Success" | "Wrong username or password",
        id?: number,
        token?: string,
    }
```
