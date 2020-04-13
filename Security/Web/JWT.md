# JWT

JWT is short for "JSON Web Access Token" pronounced as "jot" is a standard, to let a client access a resource. JWT's main components look like this:

```text
eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9. eyJzdWIiOiIxMjM0NTY3ODkwIiwibmFtZSI6IkpvaG4gRG9lIiwiYWRtaW4iOnRydWV9. TJVA95OrM7E2cBab30RMHrHDcEfxjoYZgeFONFh7HgQ
```
It is encoded by using `base64Encode()` that when is decoded looks like this:

```json
{
    "alg": "HS256",
    "typ": "JWT",
    "otherKey": "someValue"
}
```

`alg` - Stands for the algorithm used 