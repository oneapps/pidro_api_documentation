# API Documentation

* [PidroApi.UserController](#pidroapiusercontroller)
  * [users](#pidroapiusercontrollerusers)

## PidroApi.UserController
### PidroApi.UserController.users
#### GET /v2/users?username=marcelfahle returns success JSON if user is found
##### Request
* __Method:__ GET
* __Path:__ /v2/users?username=marcelfahle
##### Response
* __Status__: 200
* __Response headers:__
```
content-type: application/json; charset=utf-8
cache-control: max-age=0, private, must-revalidate
x-request-id: otc93tm1jp3bc8a8j8ptig3vjcbrlgr1
```
* __Response body:__
```json
{
  "Response": {
    "Status": 1,
    "Error": false
  }
}
```

#### GET /v2/users?username=blubb returns status 0 if user does not exist
##### Request
* __Method:__ GET
* __Path:__ /v2/users?username=blubb
##### Response
* __Status__: 200
* __Response headers:__
```
content-type: application/json; charset=utf-8
cache-control: max-age=0, private, must-revalidate
x-request-id: d42u04toe1gpr95emm31b3bcqcr63u9l
```
* __Response body:__
```json
{
  "Response": {
    "Status": 0,
    "Error": false
  }
}
```

#### GET /v2/users without params returns JSON error
##### Request
* __Method:__ GET
* __Path:__ /v2/users
##### Response
* __Status__: 404
* __Response headers:__
```
content-type: application/json; charset=utf-8
cache-control: max-age=0, private, must-revalidate
x-request-id: 5kogk7gdop8nfoltpk8hnceg5523e74i
```
* __Response body:__
```json
{
  "errors": {
    "detail": "Page not found"
  }
}
```

