[Cards for testing purpose](https://docs.adyen.com/development-resources/testing/test-card-numbers "https://docs.adyen.com/development-resources/testing/test-card-numbers")

---
There was a technical error. This test card simulates a timeout during the 3D Secure 2 authentication flow on the issuer side. Depending on your configuration, the transaction might still proceed to a successful authorization.  
5201 2829 9900 5515 03/2030 737

CloseAccount 5454 5415 8031 1093 03/2030

---

Mastercard  
2222 4000 7000 0005  
03/2030  
737

5555 3412 4444 1115  
security code optional  
03/2030  
737

5577 0000 5577 0004  
03/2030  
737

5555 4444 3333 1111  
03/2030  
737

Visa  
4111 1111 4555 1142  
security code optional  
03/2030  
737

4111 1120 1426 7661  
eight-digit BIN  
Debit  
12/2030  
737

4988 4388 4388 4305  
03/2030  
737

4166 6766 6766 6746  
03/2030  
737
___
## Check-list:

1. Transaction flow
    1. Success transaction
    2. Console message
    3. Message to user
    4. Invalid Date of Card
    5. Invalid CVV
2. Require info transmit
    1. Precisse
    2. Date format
    3. There aren't dubplicates
3. Cancel transaction
    1. Message to User
4. Perfomace testing (_Transactions that take too long to process can lead to user and potential revenue loss. Payment systems should be designed with scalability and performance in mind. Regular testing and optimization can help ensure payment processing speed and efficiency_).
5. Security
6. 3D Secure
    - ввод валидного кода из смс – успешная оплата
    - ввод невалидного кода из смс – не успешная оплата
    - ввод кода из смс после истечения времени на повторную отправку кода
    - повторный запрос кода и ввод: нового кода/предыдущего кода из смс
    - вернуться на предыдущий экран (экран ввода данных карты)
7. Main case
    - пользователь производит оплату товара
    - пользователь переходит на экран оплаты, возвращается обратно и изменяет количество товаров
    - корректный расчет комиссии
    - переход на экран оплаты с отключенным соединением с интернетом – корректное отображение ошибки
    - Currency support (_Supporting multiple currencies can be a key factor in expanding a business's customer base. Depending on the payment system, however, it can be complex due to fluctuations in exchange rates and varying compliance requirements across different regions. It's important to ensure compatibility with the currencies used by your audience and be able to update currency rates in real-time easily_).
8. Success flow
    - успешное заполнение всех необходимых полей на виджете оплаты
    - успешная оплата полной стоимости
9. Unsecessfull flow
    - плата данным платежным средством отклонена по неизвестным причинам
    - истек срок действия банковской карты
    - платеж заблокирован из-за подозрения в мошенничестве
    - не хватает денег для оплаты (сумма на карте равна нулю)
    - не хватает денег для оплаты (сумма на карте в минусе)
    - не хватает денег для оплаты (сумма на карте меньше стоимости)
    - неправильно указан номер карты
    - организация, выпустившая платежное средство, недоступна
    - исчерпан лимит платежей для данного платежного средства или вашего магазина
    - запрещены операции данным платежным средством (например, карта заблокирована из-за утери, кошелек — из-за взлома мошенниками)
    - нельзя заплатить банковской картой, выпущенной в этой стране
    - неправильно указан код CVV2 (CVC2, CID)
10. User experience (_Payment systems are often the last touchpoint for customers in an online purchasing journey. Building an intuitive and seamless payment experience is important to improve customer satisfaction. Payment systems should have clear visual cues with helpful messages, pre-filled cart details, and a smooth transition to the payment method selection and checkout pages_).
11. After pay
    - проверка чека, который приходит после оплаты
    - удостовериться, что отобразился товар на экране, например, «Мои покупки»;
    - проверить уведомление на почту (например об успешной покупке, приход чека);
    - проверить цены (например оплачен был товар со скидкой, значит итоговая (оплаченная стоимость) и отображается в чеке, на экране «Мои покупки»)
    - возврат денег на ту карту, с которой была совершена оплата
12. Multi-language support (_Multi-language support can be essential for a payment system, depending on the target audience and business goals. This includes the ability to display system prompts and error messages in different languages, localized payment methods, and support the different payment regulations and tax requirements of different countries. Having multi-language support can significantly improve the user experience and reduce the potential for errors_).
13. Integration with CRM or accounting systems (_A payment system integrated with CRM or accounting systems streamlines data reconciliation and order fulfillment processes. This can help reduce manual errors and provide real-time payment and transaction data to improve business decisions. It's important to ensure that payment systems are compatible with a variety of third-party systems and can communicate effectively with each other_).