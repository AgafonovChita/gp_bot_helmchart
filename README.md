*предварительно настроить kubernetes

1. Клонировать репозиторий: <code><b> git clone https://github.com/AgafonovChita/gp_bot_helmchart.git </b></code>

2. Заполнить данные в Makefile-example и переименовать в Makefile:
<b>botAuth.token</b> - токен для телеграмм-бота, выданный bot_father
<b>botAuth.channelId</b> - id канала, за которым бот будет следить
<b>postgresql.auth.postgresPassword</<b>b> - пароль для суперюзера postgres
<b>postgresql.auth.username</b> - имя пользователя (владелец базы данных)
<b>postgresql.auth.password</b> - пароль username(владелец базы данных)
<b>postgresql.auth.database</b> - имя базы данных
*данные от сервисного аккаунта Google - service_key.json*
<b>googleSheets.Id -
googleSheets.ServiceKey.project_id -
googleSheets.ServiceKey.private_key_id - 
googleSheets.ServiceKey.private_key - /*необходимо либо убрать все "\n", либо экранировать "\\\\n"
googleSheets.ServiceKey.client_email -
googleSheets.ServiceKey.client_id -
googleSheets.ServiceKey.client_x509_cert_url - </b>

3.Выполнить команду <code>make install_chart</code>
