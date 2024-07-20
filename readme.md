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
front .env file content:
```
REACT_APP_API_BASE_URL=http://localhost:8000
REACT_APP_TELEGRAM_BOT_TOKEN=__token__
REACT_APP_GET_USER_INFO_ENDPOINT=/user/get_info/
REACT_APP_ADD_COINS_ENDPOINT=/user/add_coins/
REACT_APP_GET_USER_REFERRALS_ENDPOINT=/user/get_user_referrals/
REACT_APP_GET_USER_PARTNERS_ENDPOINT=/levels/partner_tasks/
REACT_APP_GET_USER_SOCIALS_ENDPOINT=/levels/social_tasks/
REACT_APP_EXECUTE_SWAP_ENDPOINT=/exchanger/execute_swap/
REACT_APP_EXECUTE_TRANSFER_ENDPOINT=/exchanger/execute_transfer/
REACT_APP_EXECUTE_TRANSACTIONS_ENDPOINT=/exchanger/all_transactions/

SKIP_TELEGRAM_INIT=false
TEST_USER_ID=1234568
```

# Prerun setup
1. Ask Salo for 2 ngrok tokens and 2 ngrok domains (for BE and FE)
2. Open ngrok_be.yml (set hostname as be_ngrok_domain) 
3. Open ngrok_fe.yml (set hostname as fe_ngrok_domain) 
4. Open .env (set NGROK_AUTHTOKEN_BE, NGROK_AUTHTOKEN_FE, BACKEND_URL as https:// + be_ngrok_domain, WEBAPP_URL as https:// + fe_ngrok_domain) 

# Run latest cloud builds
0. Create .env and front.env file;
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
