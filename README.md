
### <h1 align="center"  id="heading">Create Multiple Environments In Node.js</h1>
## environments 
```
 .env.development
 .env.staging 
 .env.production 
```
## package.json
```json
"scripts": {
    "start": "env-cmd -f .env.development node ./bin/www",
    "start:staging": "env-cmd -f .env.staging node ./bin/www",
    "start:production": "env-cmd -f .env.production node ./bin/www"
},
```
## development
```bash
npm start 
```

## staging
```bash
npm run start:staging 
```

## production
```bash
npm run start:production 
``` 