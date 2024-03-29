# Задача 1: API Gateway
Решение|Маршрутизация запросов|Проверка аутентификации|Терминация HTTPS
|------|:--------------------:|:---------------------:|:-------------:|
NGINX  |Да                    |Да(доп модуль)         |Да
Kong   |Да                    |Да                     |Да
AWS API Gateway|Да            |Да                     |Да

## Выбор:
В виду того, что все из предоставленных решений подходят под нужные критерии, я бы выбрал **NGINX**, т.к. уже работал с ним, это более популярное и универсальное решение и при возникновении вопросов уже достаточно много разной документации.

# Задача 2: Брокер сообщений
Решение|Кластеризация|Хран. на диске(при доставке)|Скорость работы|Разные форматы|Разделение прав|Простота
|------|:-----------:|:--------------------------:|:-------------:|:------------:|:-------------:|:-----:|
Kafka|Да|Да|Да|Да|Да|Да|
RabbitMQ|Да|Да|Да|Да|Да|Да|
Pulsar|Да|Да|Да|Да|Да|Да|

## Выбор:
В принципе предоставленные решения все подходят под требования, ключевой вопрос будет при выборе скорость работы и опять же **популярность** решения, более популярные **Kafka и RabbitMQ**, среди них немного **быстрее будет Kafka**, но с **Rabbit у меня хороший опыт** работы, поэтому если скорость не критична, я бы выбрал **Rabbit**, если отдаем предпочтении скорости, то **Kafka**.