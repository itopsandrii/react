# react

For React.
File ENV should be renamed after download on ".env" name.


Need to do additionaly: 
testdomain.com должен проксировать на другой домен, убрать warning при проверки конфигов nginx, исправить пути каталогов в docker-compose.yaml
Задание немного наляписто сделано, нужно всё привести в порядок и ещё нужно решить прооблему с закрытием порта mysql для внешнего мира

Done:
История на счет конфигов nginx, зашел в контейнер и с помощью команды nginx -c default.conf -t исправил все.
Порт для внешнего мира закрыл для sq, внешний мир имелось ввиду сеть хоста докера, тут помог EXPOSE открытие порта в для других контейнеров, но не для хоста.
С вторым редиректом на proxysite, я что-то запутался.
Убрал лишние папки из docker-compose.
