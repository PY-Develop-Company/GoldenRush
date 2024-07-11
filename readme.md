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

NGROK_AUTHTOKEN_FE=__token__
NGROK_AUTHTOKEN_BE=__token__

JWT_SIGNING_KEY=some_key

# TGBOT
BOT_TOKEN=__token__

BACKEND_URL=http://localhost:8000
WEBAPP_URL=https://localhost:3000

ADMIN_ID=111111111

CHANNEL_ID=-1111111
CHANNEL_URL=https://t.me/slug

TG_CHANNEL=https://t.me/justforcheckingone
```

# Prerun setup
1. Ask Salo for 2 ngrok tokens and 2 ngrok domains (for BE and FE)
2. Open ngrok_be.yml (set hostname as be_ngrok_domain) 
3. Open ngrok_fe.yml (set hostname as fe_ngrok_domain) 
4. Open .env (set NGROK_AUTHTOKEN_BE, NGROK_AUTHTOKEN_FE, BACKEND_URL as https:// + be_ngrok_domain, WEBAPP_URL as https:// + fe_ngrok_domain) 

# Run latest cloud builds
0. Create .env file;
1. Open DockerDesktop;
2. Ask backend and frontend developer to push latest changes to cloud;
3. Run ```docker-compose up```

# Run local image
1. Build needed image
2. Find name of new image (the one you build) at DockerDesctop
3. Switch name of the image in docker-compose.yaml
if you are frontend developer:\
![alt text](image.png)
4. Run ```docker-compose up```
