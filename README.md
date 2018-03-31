# Django Boilerplate

## Production Environment

Main terminal:

```bash
docker-compose -f docker-compose.prod.yml build
docker-compose -f docker-compose.prod.yml up
```

Separate terminal:

```bash
# Generate backend static files.
docker exec -it backend sh -c "python manage.py collectstatic"
```
