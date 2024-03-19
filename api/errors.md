# Errors

## 401

A 401 status code is returned if there is no authentication token included in the request headers.

```typescript
401 'Unauthenticated request. Must authenticate to access API'
```

## 403

A 403 status code is returned if there is a misconfigured authentication token in the request headers.

```typescript
403 'Forbidden request. Request is incorrectly configured for authorization.'
```

## 404

A 404 status code is returned if the requested domain is not currently being tracked within the dAppling database.

```typescript
404 'Not Found'
```



:cactus:_Fun Fact: Caffeine, which naturally occurs in coffee plants, serves as a pesticide to deter herbivores from eating them._
