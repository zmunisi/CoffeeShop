# Coffee Shop Full Stack

## Full Stack Nano - IAM Final Project

Udacity has decided to open a new digitally enabled cafe for students to order drinks, socialize, and study hard. But they need help setting up their menu experience.

You have been called on to demonstrate your newly learned skills to create a full stack drink menu application. The application must:

1. Display graphics representing the ratios of ingredients in each drink.
2. Allow public users to view drink names and graphics.
3. Allow the shop baristas to see the recipe information.
4. Allow the shop managers to create new drinks and edit existing drinks.

## Tasks

There are `@TODO` comments throughout the project. We recommend tackling the sections in order. Start by reading the READMEs in:

1. [`./backend/`](./backend/README.md)
2. [`./frontend/`](./frontend/README.md)

## About the Stack

We started the full stack application for you. It is designed with some key functional areas:

### Backend

The `./backend` directory contains a partially completed Flask server with a pre-written SQLAlchemy module to simplify your data needs. You will need to complete the required endpoints, configure, and integrate Auth0 for authentication.

`@TODO` Tasks done here:
- Added Auth0 functionality
- Implemented RESTful endpoints
- Implemented error handlers
- Used [PEP8](https://www.python.org/dev/peps/pep-0008/) to enforce python code style

[View the README.md within ./backend for more details.](./backend/README.md)

### Frontend

The `./frontend` directory contains a complete Ionic frontend to consume the data from the Flask server. You will only need to update the environment variables found within (./frontend/src/environment/environment.ts) to reflect the Auth0 configuration details set up for the backend app.

`@TODO` Tasks done here:
- Added the Auth0 variables on environment.ts file
- Checked that the frontend can be launched upon with ionic serve command
- Checked and generated the login and tokens for the Barista and Manager

[View the README.md within ./frontend for more details.](./frontend/README.md)

## Auth0 account
```bash
AUTH0_DOMAIN = 'zmunisi.us.auth0.com'
ALGORITHMS = ['RS256']
API_AUDIENCE = 'coffeeshop'
```
## Created Users used to generate the Access Tokens
Since the tokens expire these two fake accounts were used to create the access tokens and saved with the latest [POSTMAN](./backend/udacity-fsnd-udaspicelatte.postman_collection.json) collection

### Barista
```bash
barista@zyhdi-munisi.com
!BrianFlanagan88
```

```bash
eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCIsImtpZCI6IjZzekhlcDNOWktQN2FNdTJZZFV5biJ9.eyJpc3MiOiJodHRwczovL3ptdW5pc2kudXMuYXV0aDAuY29tLyIsInN1YiI6ImF1dGgwfDYwYTkwNDkzZjhkMmMxMDA2YWNkYzZhMiIsImF1ZCI6ImNvZmZlZXNob3AiLCJpYXQiOjE2MjE3NzQ4NzAsImV4cCI6MTYyMTc5NjQ3MCwiYXpwIjoiazhyOHBENlphSnpwSlZCUmcwcXV1dEx3MXMxTEU4OE4iLCJzY29wZSI6IiIsInBlcm1pc3Npb25zIjpbImdldDpkcmlua3MiLCJnZXQ6ZHJpbmtzLWRldGFpbCJdfQ.23kfkmjJtuWJdR-sN4bI4fR_B0xO34myRsgQ5Ze6xRwc5igfhqbsPqZxbX3dsLEPm8mAmhQaEIgCme5xH6j5GxTXpjkc57OUfsyzhsIjFX1QJchW0NxKJ514HT-dzXlfXZxlqfL5jzvGVwH5aq5VNG9BLzWtg3n4aCLZHowjF5SIWUTyqvHrwg8vGKIJ9syCGOVsMNxnVAQxdRa-QwdQvL2hm5EwlSoh0pFv_2Zy4DAQrV-ySjlvLd927JWmcqN52kSrgdtxD8B8sNB-DYZgTdLbX3iUp1WAxpfWVIWWmRs75ZG27veZk_34yTSqc9LoIMQKgjgrN3UnxjsPjm1qJw
```

The [countdown](https://timestamp.online/countdown/1621796470) to this barista access token

### Manager
```bash
manager@zyhdi-munisi.com
!DougCoughlin88
```

```bash
eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCIsImtpZCI6IjZzekhlcDNOWktQN2FNdTJZZFV5biJ9.eyJpc3MiOiJodHRwczovL3ptdW5pc2kudXMuYXV0aDAuY29tLyIsInN1YiI6ImF1dGgwfDYwYTkwNGQ4MDFkYjQyMDA3MWFiNDhhMiIsImF1ZCI6ImNvZmZlZXNob3AiLCJpYXQiOjE2MjE3NzQ5NTcsImV4cCI6MTYyMTc5NjU1NywiYXpwIjoiazhyOHBENlphSnpwSlZCUmcwcXV1dEx3MXMxTEU4OE4iLCJzY29wZSI6IiIsInBlcm1pc3Npb25zIjpbImRlbGV0ZTpkcmlua3MiLCJnZXQ6ZHJpbmtzIiwiZ2V0OmRyaW5rcy1kZXRhaWwiLCJwYXRjaDpkcmlua3MiLCJwb3N0OmRyaW5rcyJdfQ.TcvFVK3RRri9uXBtiXhyFtFFdiu5VoQ_GF1bbYG8gc2Hw_EW1fecj12JvT-M6Bt_P5bhqZR4yuayJ3KGTx1SLt0fj8M8TtkZGRi-O8z3Zz6370X_7BBXUZe-MTcNz84z8BOAfcNFDfE1_65yvqymtRWpjNa8cHUlGRgb_AOTDRxK23hGkHu3YuTu0SLXVcrtAbBy6rt4ubLPc19r2EaXpZl8RlrvKIwkelZL8mXPGwaUnQZmjokBiqWsG3r8ubr9X5mdFXT_Cv_XdDZeZNWJMhFw2PR3IXOQdDPgfS18snW9FB3NvexoVwvS4EPT85gxtY8Pe8RtP2ZP9DUAqEcu7Q
```

The [countdown](https://timestamp.online/countdown/1621796557) to this manager access token