<font size="8">

*предварительно настроить kubernetes

1. Клонировать репозиторий: <code><b> git clone https://github.com/AgafonovChita/gp_bot_helmchart.git </b></code>

2. Заполнить данные в Makefile-example и переименовать в Makefile:
<p>
<b>botAuth.token</b> - токен для телеграмм-бота, выданный bot_father
<p>
<b>botAuth.channelId</b> - id канала, за которым бот будет следить
<p>
<b>postgresql.auth.postgresPassword</b> - пароль для суперюзера postgres
<p>
<b>postgresql.auth.username</b> - имя пользователя (владелец базы данных)
<p>
<b>postgresql.auth.password</b> - пароль username(владелец базы данных)
<p>
<b>postgresql.auth.database</b> - имя базы данных
<p>
<p>
*данные от сервисного аккаунта Google - service_key.json*
<p>
<b>googleSheets.Id -
<p>
googleSheets.ServiceKey.project_id -
<p>
googleSheets.ServiceKey.private_key_id - 
<p>
googleSheets.ServiceKey.private_key - </b>/*необходимо либо убрать все "\n", либо экранировать "\\\\n"
<b>
<p>
googleSheets.ServiceKey.client_email -
<p>
googleSheets.ServiceKey.client_id -
<p>
googleSheets.ServiceKey.client_x509_cert_url - </b>
<p>

3.Выполнить команду <code>make install_chart</code>
  
</font>
