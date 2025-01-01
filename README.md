**Домашнее задание к занятию «2.4. BDD»**

***Задача №1: Page Object's***
Вам необходимо добить тестирование функции перевода с карты на карту. Разработчики пока реализовали возможность перевода только между своими картами, но уже хотят, чтобы вы всё протестировали.

Для этого они не поленились и захардкодили вам целого одного пользователя с двумя дебетовыми картами:

* login: 'vasya'
* password: 'qwerty123'
* verification code (hardcoded): '12345'
* cards:
    * first:
        * number: '5559 0000 0000 0001'
        * balance: 10 000 RUB
    * second:
        * number: '5559 0000 0000 0002'
        * balance: 10 000 RUB
  
  После логина, который уже мы сделали на лекции, вы получите список карт.
  Нажав на кнопку «Пополнить», вы перейдёте на страницу перевода средств.

  При успешном переводе вы вернётесь назад на страницу со списком карт.

Это ключевой кейс, который нужно протестировать.

Нужно, чтобы вы через Page Object's добавили доменные методы:

получения баланса по карте со страницы списка карт,
выбора карты для пополнения,
перевода с определённой карты на выбранную карту произвольной суммы.
При этом нужно помнить, что в шаблоне Page Object's принято для описания каждой страницы сайта реализовывать отдельный класс.

Вы можете познакомиться с некоторыми подсказками по реализации [этой задачи](https://github.com/netology-code/aqa-homeworks/blob/master/bdd/balance.md).