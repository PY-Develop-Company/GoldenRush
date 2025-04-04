# 🇺🇸 (EN)
## ☁️Run cloud project
1. Create an .env file with the contents:
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

TRANSFER_FEE_PERCENTAGE=3
VIP_PRICE=100

FAIRY_GIFT_SHOW_INTERVAL=600

USDT_PAYOUT_MINIMUM_RANK=7

CRYPTOPAY_TOKEN=__token__
CRYPTOPAY_BASE_URL=https://pay.crypt.bot/api/
CRYPTOPAY_TG_LINK=https://t.me/CryptoBot
CRYPTOPAY_TG_TAG=@CryptoBot

# TGBOT
BOT_TOKEN=__token__

BACKEND_URL=http://localhost:8000
WEBAPP_URL=https://localhost:3000

ADMIN_ID=111111111

CHANNEL_ID=-1111111
CHANNEL_URL=https://t.me/slug
TG_CHANNEL=https://t.me/justforcheckingone

MAILING_GROUP_SIZE=20
MAILING_GROUP_INTERVAL=20
MAILING_AVAILABLE_LANGUAGES=uk,ru,en
```
2. Create a front.env file with the contents:
```
REACT_APP_API_BASE_BASE_URL=http://localhost:8000
REACT_APP_API_BASE_NOPROTOCOL_URL=localhost:8000
REACT_APP_TELEGRAM_BOT_TOKEN=__token__

REACT_APP_GET_USER_INFO_ENDPOINT=/user/get_info/
REACT_APP_ADD_COINS_ENDPOINT=/user/register_clicks/
REACT_APP_GET_USER_REFERRALS_ENDPOINT=/user/get_user_referrals/
REACT_APP_GET_FREN_LINK_ENDPOINT=/user/fren_link/
REACT_APP_GET_USER_PARTNERS_ENDPOINT=/levels/partner_tasks/
REACT_APP_GET_USER_SOCIALS_ENDPOINT=/levels/social_tasks/
REACT_APP_EXECUTE_SWAP_ENDPOINT=/exchanger/execute_swap/
REACT_APP_EXECUTE_TRANSFER_ENDPOINT=/exchanger/execute_transfer/
REACT_APP_EXECUTE_TRANSACTIONS_ENDPOINT=/exchanger/all_transactions/
REACT_APP_UPDATE_SETTINGS_ENDPOINT=/user/update_settings/
REACT_APP_GET_ALL_ACTIVE_BANNER_ADVERTS_ENDPOINT=/ads/all_active_relevant_banner_adverts/
REACT_APP_GET_RANDOM_FULLSCREEN_BANNER_ADVERTS_ENDPOINT=/ads/get_relevant_random_fullscreen_advert/
REACT_APP_TRACK_BANNER_ADVERTS_ENDPOINT=/ads/track_banner_ad/
REACT_APP_GIVE_ADVIEW_REWARD_ENDPOINT=/ads/give_adview_reward/
REACT_APP_CHECK_PARTNER_TASK_ENDPOINT=/levels/check_partner_task/
REACT_APP_CHECK_SOCIALS_TASK_ENDPOINT=/levels/check_social_task/
REACT_APP_GET_TRANSFER_FEE_ENDPOINT=/exchanger/get_transfer_fee/
REACT_APP_CREATE_INVOICE_ENDPOINT=/exchanger/create_invoice/
REACT_APP_CHECK_INVOICE_ENDPOINT=/exchanger/check_invoice_status/
REACT_APP_CRYPTO_TRANSFER_ENDPOINT=/exchanger/crypto_transfer/
REACT_APP_GET_ALL_REGIONS=/user/all_regions/
REACT_APP_CREATE_ADSET=/ads/create_adset/
REACT_APP_GET_USER_ADSETS=/ads/all_user_adsets/
REACT_APP_GET_BANNER_ADVERT=/ads/get_banner_advert/
REACT_APP_GET_FULLSCREEN_ADVERT=/ads/get_fullscreen_advert/
REACT_APP_CREATE_BANER_ADVERT=/ads/create_banner_ad/
REACT_APP_CREATE_FULLSCREEN_ADVERT=/ads/create_fullscreen_ad/
REACT_APP_ENABLE_ADSET=/ads/enable_adset/
REACT_APP_DISABLE_ADSET=/ads/disable_adset/
REACT_APP_ADD_DELETE_ADSET=/ads/delete_adset/
REACT_APP_CANSELL_SHUTDOWN=/ads/cancel_adset_disabling/
REACT_APP_GET_EXCHANGER_RATE_ENDPOINT=/exchanger/get_exchange_rate/
REACT_APP_BY_VIP_RATE_ENDPOINT=/exchanger/buy_vip/
REACT_APP_UPDATE_LAST_ACTIVE=/user/update_last_active/
REACT_APP_EXECUTE_GAMELIST=/api/mini_games_app/
REACT_APP_GAME1_MONEY=/api/mini_games_app/fortune
REACT_APP_GAME1_START=/api/mini_games_app/fortune/start
REACT_APP_GAME1_RESULT=/api/mini_games_app/fortune/result
REACT_APP_GAME2_MONEY=/api/mini_games_app/sapper
REACT_APP_GAME2_START=/api/mini_games_app/sapper/start
REACT_APP_GAME2_RESULT=/api/mini_games_app/sapper/result
REACT_APP_GAME3_WEBS=/ws/minigames/crash/
REACT_APP_GAME3_MAKEBET=/api/mini_games_app/crash/make_bet
REACT_APP_GAME3_TAKEBET=/api/mini_games_app/crash/pick_up_bet
REACT_APP_GAME4_MAKEBET=/api/mini_games_app/graph/make_bet
REACT_APP_GAME4_CHECKGAME=/api/mini_games_app/graph/is_user_in_game
REACT_APP_GAME4_PERSONAL_GAME=/ws/minigames/graph/personalgame
REACT_APP_GAME4_GETBTCPRICE=/api/mini_games_app/graph/get_cost_btc
REACT_APP_GAME4_GET_LAST_GAME=/api/mini_games_app/graph/get_last_info_game
REACT_APP_GAME4_LINKS=/api/mini_games_app/graph/links
REACT_APP_GAME4_WEBS=/ws/minigames/graph/
REACT_APP_GAME4_WEBS2=/ws/minigames/graph/costbtc/
REACT_APP_GAME4_GETBTCPRICE=/api/mini_games_app/graph/get_cost_btc
REACT_APP_GAME5_MONEY=/api/mini_games_app/football
REACT_APP_GAME5_WEBS=/ws/minigames/football/
REACT_APP_GAME5_START=/api/mini_games_app/football/start
REACT_APP_GAME5_END=/api/mini_games_app/football/end
REACT_APP_PICK_GENDER=/user/pick_gender/
REACT_APP_LEVEL_NEXT_RANK=/levels/next_rank/
REACT_APP_GET_USER_CURRENT_STAGE_INFO=/levels/get_user_current_stage_info/
REACT_APP_CLAIM_TASK=/levels/claim_task/
REACT_APP_BUY_TASK=/levels/buy_task/
REACT_APP_BUY_ROAD=/levels/buy_road/
REACT_APP_GET_USER_CURRENT_RANK_INFO=/levels/get_user_current_rank_info/
REACT_APP_NEXT_STAGE=/levels/next_stage/

REACT_APP_SKIP_TELEGRAM_INIT=false
REACT_APP_TEST_USER_ID=123456
```
front_admin.env
```
REACT_APP_API_BASE_BASE_URL=http://localhost:8000
REACT_APP_LOGIN_ENDPOINT=/ads/admin_login/
REACT_APP_GET_ADVERTS_ENDPOINT=/ads/verification_requests/
REACT_APP_VERIFICATION_ENDPOINT=/ads/handle_advert_verification_request/
REACT_APP_GET_INVITERS_ENDPOINT=/api/stats/get-all-inviters/
REACT_APP_GET_GAME_STATS=/api/stats/get-game-stats/
REACT_APP_GET_ALL_INVOICES=/api/stats/get-all-invoices
```
3. Ask Salo for 2 ngrok tokens and 2 ngrok domains (for BE and FE);
4. Open ngrok_be.yml (set hostname as be_ngrok_domain);
5. Open ngrok_fe.yml (set hostname as fe_ngrok_domain);
6. Open .env (set NGROK_AUTHTOKEN_BE, NGROK_AUTHTOKEN_FE, BACKEND_URL as https:// + be_ngrok_domain, WEBAPP_URL as https:// + fe_ngrok_domain)
7. Ask backend and frontend and tg-bot developers to push latest changes to cloud;
8. Open DockerDesktop;
9. Run the command 
```
docker-compose up
```

## 🏠Run local image
1. Create the image;
2. Find the image name in DockerDesktop;
3. Set the image name in docker-compose.yaml
if you are a frontend developer, then this line:\
![alt text](image.png)
4. Run the command
```
docker-compose up
```

## How to deploy
1. Enter vilors Dedicated Server
2. Enter directory Documents/GitHub/GoldenRush/
```
cd Documents/GitHub/GoldenRush/
```
3. Stop Docker containers
```
sudo docker-compose down
```
4. Delete volume with db data
```
sudo docker volume rm goldenrush_dev-db-data
```
5. Pull new images from cloud. If frontend changed:
```
sudo docker pull alexk0valchuk/bwgcombat:frontend
```
6. Change .env or front.env file if needed:
```
sudo nano .env
```
```
sudo nano front.env
```
6. Run the app
```
sudo docker-compose up
```

# 🇺🇦 (UA)
## ☁️Запустити хмарний проект
1. Створити файл .env з вмістом:
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

NGROK_AUTHTOKEN_FE=__token___
NGROK_AUTHTOKEN_BE=__token___

JWT_SIGNING_KEY=деякий_ключ

# TGBOT
BOT_TOKEN=__token__

BACKEND_URL=http://localhost:8000
WEBAPP_URL=https://localhost:3000

ADMIN_ID=111111111

CHANNEL_ID=-1111111
CHANNEL_URL=https://t.me/slug

TG_CHANNEL=https://t.me/justforcheckingone
```
2. Створіть файл front.env із вмістом:
```
REACT_APP_API_BASE_BASE_URL=http://localhost:8000
REACT_APP_TELEGRAM_BOT_TOKEN=__token__
REACT_APP_GET_USER_INFO_ENDPOINT=/user/get_info/
REACT_APP_ADD_COINS_ENDPOINT=/user/add_coins/
REACT_APP_GET_USER_REFERRALS_ENDPOINT=/user/get_user_referrals/
REACT_APP_GET_USER_PARTNERS_ENDPOINT=/levels/partner_tasks/
REACT_APP_GET_USER_SOCIALS_ENDPOINT=/levels/social_tasks/
REACT_APP_EXECUTE_SWAP_ENDPOINT=/exchanger/execute_swap/
REACT_APP_EXECUTE_TRANSFER_ENDPOINT=/exchanger/execute_transfer/
REACT_APP_EXECUTE_TRANSACTIONS_ENDPOINT=/exchanger/all_transactions/

REACT_APP_SKIP_TELEGRAM_INIT=false
REACT_APP_TEST_USER_ID=123568
```
3. Попросіть у Salo 2 токени ngrok і 2 домени ngrok (для BE і FE);
4. Відкрийте ngrok_be.yml (задайте hostname як be_ngrok_domain);
5. Відкрийте ngrok_fe.yml (задайте hostname як fe_ngrok_domain);
6. Відкрити .env (встановити значення змінних NGROK_AUTHTOKEN_BE, NGROK_AUTHTOKEN_FE, BACKEND_URL як https:// + be_ngrok_domain, WEBAPP_URL як https:// + fe_ngrok_domain)
7. Попросіть розробників бекенду, фронтенду та tg-ботів перенести останні зміни в хмару;
8. Відкрийте DockerDesktop;
9. Запустіть проект за допомогою команди 
```
docker-compose up
```

## 🏠Запустити локальний image
1. Створіть image;
2. Знайдіть назву image у DockerDesktop;
3. Змініть ім'я image в файлі docker-compose.yaml
якщо ви фронтенд-розробник, то цей рядок:\
![alt text](image.png)
4. Запустіть проект за допомогою команди 
```
docker-compose up
```

## Як задеплоїти проект
1. Увійдіть у віддалений сервер vilors
2. Увійдіть в папку/директорію Documents/GitHub/GoldenRush/
```
cd Documents/GitHub/GoldenRush/
```
3. Зупиніть Docker контейнери
```
sudo docker-compose down
```
4. Видаліть volume з інформацією бази даних
```
sudo docker volume rm goldenrush_dev-db-data
```
5. Зтягніть зміни image з хмари. Якщо зміни фронту:
```
sudo docker pull alexk0valchuk/bwgcombat:frontend
```
6. Змініть .env або front.env файли якщо потрібно:
```
sudo nano .env
```
```
sudo nano front.env
```
6. Запустити програму
```
sudo docker-compose up
```