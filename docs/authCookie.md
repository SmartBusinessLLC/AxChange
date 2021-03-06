# Cookie authorization

Даний тип авторизації потребує даних про `cookie` для авторизації в сервісі з яким відбувається обмін даними. Отримання `cookie` відбувається зарахунок створення ще одного запиту, наприклад з іншими типом авторизації. Отримані від іншого запиту заголовки у відповіді, обробляються і значення ключа `Set-Cookie` встановлюється системою автоматично в заголовки запиту.

![](../_media/requestParameter_8.png)

!> Поле `Request for auth` може мати значення запитів, що є `Only for internal`. Обрати в якості значення нинішній запит неможливо.

Якщо для запиту поле `Make history` встановлено в значення `Так`, тоді при використанні іншого запиту для отримання даних для авторизації, для цього запису історія буде створена в рамках його налаштувань. Наприклад:

```text
'Request A' uses 'Request B'
'Request A' do not make history
'Request B' make history

When 'Request A' will be invoked, history will be created only for 'Request B'
```
