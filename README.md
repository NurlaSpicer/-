# -File post request:
http://localhost:8080/api/file/upload
curl -X 'POST' \
  'http://localhost:8080/api/file/upload' \
  -H 'accept: */*' \
  -H 'Content-Type: application/json' \
  -d '{
  "file": "app"
}'

# File get request:
curl -X 'GET' \
  'http://localhost:8080/api/file/1' \
  -H 'accept: */*'
http://localhost:8080/api/file/1


# Product post request:
http://localhost:8080/api/product/create?productName=apple&price=100&fileID=1&available=true
curl -X 'POST' \
  'http://localhost:8080/api/product/create?productName=apple&price=100&fileID=1&available=true' \
  -H 'accept: */*' \
  -d '
http://localhost:8080/api/product

# Product put request:
http://localhost:8080/api/product
curl -X 'PUT' \
  'http://localhost:8080/api/product' \
  -H 'accept: */*' \
  -H 'Content-Type: application/json' \
  -d '{
  "id": 1,
  "productName": "",
  "price": 0,
  "fileID": 0,
  "available": false
}'

# Product get request:
http://localhost:8080/api/product
curl -X 'GET' \
  'http://localhost:8080/api/product' \
  -H 'accept: */*'
curl -X 'GET' \
  'http://localhost:8080/api/product/1' \
  -H 'accept: */*'

http://localhost:8080/api/product/1
curl -X 'GET' \
  'http://localhost:8080/api/product/1' \
  -H 'accept: */*'

http://localhost:8080/api/product/findByVersion/1
curl -X 'GET' \
  'http://localhost:8080/api/product/findByVersion/1' \
  -H 'accept: */*'

http://localhost:8080/api/product/findByProductName/apple
curl -X 'GET' \
  'http://localhost:8080/api/product/findByProductName/apple' \
  -H 'accept: */*'

http://localhost:8080/api/product/findByPrice/100
curl -X 'GET' \
  'http://localhost:8080/api/product/findByPrice/100' \
  -H 'accept: */*'

# Product delete request:
http://localhost:8080/api/product/1
curl -X 'DELETE' \
  'http://localhost:8080/api/product/1' \
  -H 'accept: */*'


# Category post request:
http://localhost:8080/api/category/create?categoryName=Fruits&productsID=1
curl -X 'POST' \
  'http://localhost:8080/api/category/create?categoryName=Fruits&productsID=1' \
  -H 'accept: */*' \
  -d ''

# Category put request:
http://localhost:8080/api/category
curl -X 'PUT' \
  'http://localhost:8080/api/category' \
  -H 'accept: */*' \
  -H 'Content-Type: application/json' \
  -d '{
  "id": 1,
  "categoryName": "Fruit",
  "productsID": [
    1
  ]
}'

# Category get request:
http://localhost:8080/api/category
curl -X 'GET' \
  'http://localhost:8080/api/category' \
  -H 'accept: */*'

http://localhost:8080/api/category/1
curl -X 'GET' \
  'http://localhost:8080/api/category/1' \
  -H 'accept: */*'

# Category delete request:
http://localhost:8080/api/category/1
curl -X 'DELETE' \
  'http://localhost:8080/api/category/1' \
  -H 'accept: */*'


# Stock post request:
http://localhost:8080/api/stock/create?stockName=Ex&typeName=pipeline
curl -X 'POST' \
  'http://localhost:8080/api/stock/create?stockName=Ex&typeName=pipeline' \
  -H 'accept: */*' \
  -d ''

# Stock put request:
http://localhost:8080/api/stock
curl -X 'PUT' \
  'http://localhost:8080/api/stock' \
  -H 'accept: */*' \
  -H 'Content-Type: application/json' \
  -d '{
  "id": 1,
  "stockName": "Avagard",
  "typeName": "",
  "productsID": [
    1
  ]
}'

# Stock get request:
http://localhost:8080/api/stock
curl -X 'GET' \
  'http://localhost:8080/api/stock' \
  -H 'accept: */*'

http://localhost:8080/api/stock/1
curl -X 'GET' \
  'http://localhost:8080/api/stock/1' \
  -H 'accept: */*'

# Stock delete request:
http://localhost:8080/api/stock/1
curl -X 'DELETE' \
  'http://localhost:8080/api/stock/1' \
  -H 'accept: */*'


# User post request:
http://localhost:8080/api/user/create?userName=Nurla&password=123qwerty&role=admin
curl -X 'POST' \
  'http://localhost:8080/api/user/create?userName=Nurla&password=123qwerty&role=admin' \
  -H 'accept: */*' \
  -d ''


# User put request:
http://localhost:8080/api/user
curl -X 'PUT' \
  'http://localhost:8080/api/user' \
  -H 'accept: */*' \
  -H 'Content-Type: application/json' \
  -d '{
  "id": 1,
  "userName": "",
  "password": "",
  "role": "",
  "productsID": [
    1
  ]
}'


# User get request:
http://localhost:8080/api/user
curl -X 'GET' \
  'http://localhost:8080/api/user' \
  -H 'accept: */*'

http://localhost:8080/api/user/options
curl -X 'OPTIONS' \
  'http://localhost:8080/api/user/options' \
  -H 'accept: */*'

http://localhost:8080/api/user/1
curl -X 'GET' \
  'http://localhost:8080/api/user/1' \
  -H 'accept: */*'

http://localhost:8080/api/user/header
curl -X 'GET' \
  'http://localhost:8080/api/user/header' \
  -H 'accept: */*' \
  -H 'name: asd'

http://localhost:8080/api/user/findByUserName/Nurla
curl -X 'GET' \
  'http://localhost:8080/api/user/findByUserName/Nurla' \
  -H 'accept: */*'

http://localhost:8080/api/user/findByRoleName/ROLE_ADMIN
curl -X 'GET' \
  'http://localhost:8080/api/user/findByRoleName/ROLE_ADMIN' \
  -H 'accept: */*'

# User delete request:
http://localhost:8080/api/user/1
curl -X 'DELETE' \
  'http://localhost:8080/api/user/1' \
  -H 'accept: */*'
