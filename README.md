# MineServ-Rewards-LLSE
Плагин системы поощрений игроков мониторинга MineServ, работающий с LiteLoader ScriptEngine для Minecraft Bedrock.
Данный плагин поможет вам реализовать поощрения для игроков без лишней возни с вебсервером и RCON. Всё, что вам нужно сделать - установить данный плагин на ваш сервер.
Установить плагин - очень просто. Всё, что вам нужно сделать - скачать файл `RewardSystemLLSE.llplugin` из [**релизов**](https://github.com/mineserv-top/RewardSystemLLSE/releases/) и поместить его в папку `plugins` вашего сервера.
Далее вам нужно настроить плагин. Пример Конфигурации с описаниями перемунных вы можете увидеть ниже -

```json
{
    "WebServerPort": "8080",//Порт веб сервера, который будет использоваться для связи мониторинга с этим плагином. На странице редактирования провета нужно будет вводить "http://ip:port", в данном случае IP - IP сервера, а порт - порт веб сервера, который вы указали тут. Важно: порт должен быть открыт в фаерволе!
    "SecretKey": "",//Секретный ключ, который можно получить на странице редактирования проекта
    "LiteLoader": {
        "Command1":"give $user diamond",//Первая команда, которая будет исполняться, когда игрок проголосует. Если стоит null, то команда выполнена не будет.
        "Command2":"null",//Вторая команда, которая будет исполняться, когда игрок проголосует. Если стоит null, то команда выполнена не будет.
        "Command3":"null"//Третья команда, которая будет исполняться, когда игрок проголосует. Если стоит null, то команда выполнена не будет.
        //Поддерживаются любые команды!
    }
}
```
Приятного использования!