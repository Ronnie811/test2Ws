# A simple Docker( React / Express ) App to practice CI / CD

## Frontend workflow
- cd client
- npm install
- npm start   (dev server)
- npm test    (frontend tests)
- npm build   (bundle source and send to ../server/client)

#### Requirements:
client/.env file (not version controlled): <--- Will be changing as pipeline matures<br>
REACT_APP_DEV_SERVER=localhost:3001 <br>
REACT_APP_PROD_SERVER=localhost:3001 <br>
REACT_APP_TEST_SERVER=localhost:3001

## Backend workflow
- cd server
- npm install
- npm start   (Dev server, connecting to localhost mongodb)
- npm test    (backend tests)
- npm deploy  (Production server, connecting to deployment mongodb)
