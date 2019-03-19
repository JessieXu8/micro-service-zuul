```
  path indicates that it will jump to "http://localhost:8181/" when we visit url with "/api"
  8181 is server port which already register in Eureka
  For example, we can visit "http://localhost:8000/api/item/1" instead of "http://localhost:8181/item/1"
  1. First Way
  routes:
    item:
      path: /api/**
      url: http://localhost:8181/
zuul:
  routes:
    item:
      path: /api/**
      service-id: micro-service-order
```

