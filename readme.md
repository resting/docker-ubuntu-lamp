- `html` is mounted to `/var/www/` replacing the original `/var/www/html`.

### Run
`docker run -it -p 8000:80 -p 3309:3306 -v $(pwd)/html:/var/www/html resting/ubuntu bash`