# Bookinfo Application for Workshop

This is a way to run app with docker compose it use nginx as ingress to control traffic for each services.

nginx will run on **port:9080**


### Start application and all services
```
docker compose up -d
```

### Stop application and all services
```
docker compose down
```

After run compose you can access app or services below.
- The followings are **hostname** inside Nginx Ingress route
    - productpage-service: http://productpage:9080
    - details-service: http://details:9080
    - reviews-service: http://reviews:9080
    - ratings-service: http://ratings:9080
    - db: mongodb://db:27017

<br />

- The followings are **hostname** outside use for Postman
    - productpage-service: http://localhost:9080
    - details-service: http://localhost:9080/details
    - reviews-service: http://localhost:9080/reviews
    - ratings-service: http://localhost:9080/ratings
    - db: mongodb://db:27017