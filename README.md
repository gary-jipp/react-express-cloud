
### Automated Build
- cd server, npm install
- cd client, npm install
- what if there was a way to do ALL of this in a single step?

### Modify `package.json`
- create a top-level `package.json`
- create an install for the server
- create install for the client
- exactly the same as we do manually
- test, them out
- now lets create a single `install` that does them both
- `npm install`

### Build & Deploy the React Build
- cd client, npm run build
- `build:client` script

- mv client/dist ./public
- `deploy:client` script

### Single `build` command
- Single `build` script can do everything
- npm install, npm build:client, npm deploy:client

### Run our App
- cd server, npm start
- `start` script

## Final Sequence
- `npm run build`
- `npm start`