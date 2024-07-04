.env file content:
```
DEBUG=1
DJANGO_ALLOWED_HOSTS=*

ADMIN_USERNAME=admin
ADMIN_PASSWORD=admin
ADMIN_TG_ID=987654321

DB_NAME=bwgcombat_db
DB_HOST=db
DB_USER=root
DB_PASS=root
DB_PORT=5432

NGROK_AUTHTOKEN=__token__

JWT_SIGNING_KEY=some_key
```

1. Open DockerDesktop;
2. Ask backend and frontend developer to push latest changes to cloud;
3. Run ```docekr-compose up```
