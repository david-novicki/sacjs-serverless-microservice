# sacjs-serverless-microservice
Serverless framework example for 9/26/2017 SacJS Meetup

## Install
### Install serverless
npm install -g serverless

### Pull repo
git clone https://github.com/supercycle91/sacjs-serverless-microservice.git && cd sacjs-hello-world

## Testing
### Deploy
serverless deploy -v

### Test
serverless invoke -f hello

### Run logs
serverless logs -f hello -t

### Deploy function only
serverless deploy function -f hello

### Add API gateway (add to yml)
events:
      - http:
            path: sacjs
            method: get
            cors: true

### Deploy
serverless deploy -v

### Test
curl ‘url’

## Remove all resources from AWS
### Remove
serverless remove
