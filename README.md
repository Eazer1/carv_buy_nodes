# Carv Buy Nodes
[**EN README**](https://github.com/Eazer1/carv_buy_nodes/blob/main/README_EN.md)

Carv Buy Nodes - это автоматизированный инструмент на python, предназначенный для автоматической покупки нод Carv согласно заданным пользователем характеристикам. Этот инструмент позволяет пользователям указать желаемый тир ноды и количество для покупки, а также автоматически применяет скидку 10%, которую Aethir предоставит через две недели после покупки.

Информация о проекте: https://t.me/Eazercrypto/1132


## Особенности
- Автоматическая покупка нод Carv согласно заданным характеристикам (тир и количество).
- Применение автоматической скидки 10%.
- Простота настройки и использования.
- Если у вас есть собственная нода Arbitrum, то замените в файле cfg.py значение "NODE_RPC"
- Код можно и даже желательно запустить заранее. Он проверит, хватает ли на ваших кошельках $wETH и сделает апрувы на контракты сейла нод

## Настройка

- Python 3.10

```
git clone https://github.com/Eazer1/carv_buy_nodes
```
```
cd aethir_buy_nodes
```
```
pip install -r requirements.txt
```

Загрузка в wallets.txt кошельков в формате prkey;tier;amount где:
- prkey - приватный ключ от вашего кошелька
- tier - Тир ноды, который вы планируете купить
- amount -  Количество нод, которое вы планируете купить

Есть возможность построчно загрузить более 1-го кошелька
пример:
```
0x0000000000000000000000000000000000000;1;1
0x0000000000000000000000000000000000001;14;3
0x0000000000000000000000000000000000002;53;10
```

## Примечание

### Учтите, что:

- На кошельке нужно иметь токен $wETH, а не $ETH
- Код автоматически делает approve $wETH на адрес покупки нод (не более, чем вы запланировали купить), поэтому не пугайтесь

- Код создан админом канала https://t.me/Eazercrypto
