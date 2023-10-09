## How to make app working

- Clone the repo using `git clone https://github.com/OmarAshour207/our-education.git`.
- Run `cd /our-edu` then `composer install`.
- Make copy from .env.example file called .env .
- Make new database and put the credentials in .env file.
- Run `php artisan migrate --seed`.
- Congrats it works.

# There are two endpoints for users and transactions.

## Users endpoint GET: /api/users

We can use many params to filter 

- get all the users combine with transactions using: /api/users
- get users filtered with currency using: /api/users?currency=`any allowed cuurency`

## Transactions endpoint GET: /api/transaction

There are many params using in filters.

- all transactions: /api/transactions
- transaction filtered with statusCode: /api/transactions?statusCode=`1 or 2 or 3`
- transaction filtered with statusCode: /api/transactions?currency=`any cuurency allowed`
- transaction filtered with statusCode: /api/transactions?lowAmount=`number`&highAmount=`number`
- transaction filtered with statusCode: /api/transactions?startDate=`YYYY-mm-dd`&endDate=`YYYY-mm-dd`

## Api collection link
[Our Education Collection](https://api.postman.com/collections/8536121-187f450e-292e-45a7-b392-5bc2fea155da?access_key=PMAT-01H04JHXVY3EMN7FW1M78KP3N3)
