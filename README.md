# qp-assessment
qp-assessment

1. Get groceries
curl --location 'http://0.0.0.0:5000/api/groceries/'

2. Add groceries
curl --location 'http://localhost:5000/api/groceries/add' \
--header 'Content-Type: application/json' \
--data '{
           "name": "jackfruit",
           "price": 1.2,
           "stock": 50,
           "description": "jackfruit"
         }'


3. createOrders
curl --location 'http://localhost:5000/api/orders' \
--header 'Content-Type: application/json' \
--data '{
           "items": [
             {
               "groceryId": 1740045793745,
               "quantity": 1
             }
           ]
         }'


4. get all orders
curl --location 'http://localhost:5000/api/orders'

5. delete grocery items
curl --location --request DELETE 'http://localhost:5000/api/groceries/1740045814787'