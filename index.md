# IT Hub API docs

## /users
Protected endpoint.

### GET /users
Returns an array of users

```
[
    {
        "id": "1f69ac9a-c0f0-464a-9005-f519c2d488d2",
        "authOId": "",
        "firstName": "",
        "lastName": "",
        "fullName": "",
        "createdAt": "2021-11-28T09:19:25.879Z",
        "updatedAt": "2021-11-28T09:19:25.879Z"
    },
]
```

### POST /users
Creates new user

Request:
```
{
    "firstName": "Brano",
    "lastName": "Admin",
    "authOId": "asdf9asdf9asdf9asdf"  // REQUIRED, UNIQUE
}
```

Response:
```
{
    "firstName": "Brano",
    "lastName": "Admin",
    "fullName": "Brano Admin",
    "authOId": "some-id-from-authO",
    "id": "17b90c7e-7b37-468c-a908-20a69b3f4bd9",
    "createdAt": "2021-11-28T11:02:11.226Z",
    "updatedAt": "2021-11-28T11:02:11.226Z"
}
```
