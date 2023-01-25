**Demo or Result can be accessed [brik.migun.my.id](http://brik.migun.my.id/)** <br />
**Documentation can be accessed [here](http://brik.migun.my.id/api/documentation)**

**Create product management server using nodejs (nestjs, expressjs, or other framework) with this criteria:**
<br />
**Database (Provide ERD)**
-   Table products
	-   id
	-   name
	-   description
	-   price
	-   image_url
-   Table orders
	-   id
	-   Total_price
-   Table customers
	-   id
	-   name

**API (Provide API documentation)**
-   **CRUD product**
	-   Create product API
	-   Read all products API
	-   Read product by id API
	-   Update product API
	-   Delete product API

-   **Create orders API** 
    - Body:
	    -   Array of products
	    -   Customer name
    -   Response:

        -   200
	        -  { success: true, message: ‘successfully create order’ }
        -  400
	        - { success: false, message: ‘failed to create customer’ }    

**Flow** <br />
-   Create order flow:
    1.  Create Customer
    2.  Create Orders

- Specifications:
    -   We don’t want customer without order
    -   We don’t want any order without customer

**Deploy** <br/>
-	Please deploy the server to your preferred cloud.

* If you think this design needs more table or additional flow, feel free to add those.
* feel free to use your preferred architecture 

**Point plus**
- Deploy documentation


## Description

[Brik BE Test](https://github.com/brik-id/be-test) Take Home Test from Brik.
Duplicate from [this repository](https://github.com/mgportofolio/brik-be-test)

## Installation

```bash
$ npm install
```

## Database Migration

- Copy .env.example

- Change DATABASE_URL to your Database Configuration

- Run db.sql in your database query to initialize the database

- Run this command
```bash
# Migrate
$ npx prisma migrate dev --name init

# Generate ORM
$ npx prisma generate
```

## Running the app

```bash
# development
$ npm run start

# watch mode
$ npm run start:dev

# production mode
$ npm run start:prod
```


# Detail
- Hosted in [Google Cloud Platform](https://github.com/brik-id/be-test)
- Framework: [Nest](https://github.com/brik-id/be-test)
- Database: [PostgreSQL](https://github.com/brik-id/be-test)
- Deployed: [brik.migun.my.id](http://brik.migun.my.id)
- Documentation: [brik.migun.my.id/api/documentation](http://brik.migun.my.id/api/documentation)