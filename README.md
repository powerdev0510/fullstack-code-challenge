# Code Challenge
You have 24 hours to build a simple [GraphQL](https://graphql.org/) API with a [React](https://reactjs.org/) frontend. The API must be written in Node.js (using express), and you may use the following tools/packages/libraries:

- [express](https://expressjs.com/) (server must be express)
- [apollo](https://www.apollographql.com/) (both server and client)
- [lodash](https://lodash.com/)/[underscore](https://underscorejs.org/)
- An ORM (i.e. [sequelize](http://sequelize.org/)) or SQL query builder (i.e. [knex.js](http://knexjs.org/)) of your choice
- A node Postgres library (i.e. [node-postgres](https://node-postgres.com/)) to connect with your ORM or query builder if you choose to use one
- A client side UI component library ([material-ui](https://material-ui.com/), [bootstrap](https://react-bootstrap.github.io/), etc.)

**Note:** Do not use any autogeneration libraries/frameworks such as [PostGraphile](https://www.graphile.org/postgraphile/) or [Hasura](https://hasura.io/).

## Description of Application
The application consists of **users** and **products**.

### Users
Each user must have, but is not limited to:

- ID
- First Name
- Last Name
- Email (unique)

**Please note:**

- These users are the only users that are able to make requests via the API.
- User creation/maintenance is not done through the API (see Database section below).
- Users can own many products

### Products
Each product must have, but is not limited to:

- ID
- Name
- Description
- Price
- Image

### Database
- Postgres
- All tables in the database must be created programatically
- The user table should be seeded with five (5) users

### Authentication
You must implement an authentication system so that the API knows which of the users is making the request. All requests should ensure that an authorized user is making the request. In the event of an unauthorized user, an error should be thrown.

### Requests
The following operations should be implemented:

- Add product
  - All fields required except ID and image
- Update product
  - All fields required except image
- Delete product
- Get product
- Upload product image
- Get list of all products
- Attach product to requesting user
- Remove product from requesting user
- List products attached to requesting user

### Frontend
Display a list of users with pagination. Additionally display the products a user owns in anyway you see fit.

**Please note:** The frontend does NOT need to be able to create, edit, or delete data.

### Tests
You should write tests to back up your code. You are free to use any testing tools or frameworks you like.

## Completion
When you are finished (or out of time) you will push up the application to a git repo. Then please notify Thomas Kane via email (thomas@pumpjackdataworks.com) with the subject Pumpjack Code Challenge and the link to the github repo. Please include:

- Instructions on how to create and seed database tables
- Instructions on how authentication works
- Anything else you think Thomas should know to run the application (if anything)
Thomas is available for any questions you may have via email at thomas@pumpjackdataworks.com.

![Good Luck](https://media.giphy.com/media/3ohfFopqHDT7vcMM2A/giphy.gif)
