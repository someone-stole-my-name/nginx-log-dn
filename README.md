```bash
docker run --rm -it -p 4433:443 \
    -v $(pwd)/ca:/etc/nginx/ca \
    -v $(pwd)/crt:/etc/nginx/crt \
    -v $(pwd)/key:/etc/nginx/key \
    -v $(pwd)/nginx.conf:/etc/nginx/nginx.conf \
    nginx:latest
```
