# Minimal repo based on subroute proxied by nginx

# Run service

```
yarn
yarn start:dev
```

# Run nginx
```
docker-compose up -d
```

# Test

1. ✅ Visit [http://localhost:3000/docs](http://localhost:3000/docs), swagger works expectedly.
2. ❌ Visit [http://localhost:3100/api/docs](http://localhost:3100/api/docs)(proxied by nginx on path: `/api/`), swagger not works.
