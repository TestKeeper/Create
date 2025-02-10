##  Чек лист проверки валидации блока создания позиции



#### Проверка  выбора направления позиции
    1.Проверить переключение  между вкладками Long/Short

#### Проверка  выбора типа маркета
    1.Проверить кликабельность полей Market,Limit,Stop,Stop Market
    2.Проверить что при смене типа ордера (маркет/лимит/стоп-маркет/стоп-лимит) сохраняются:
    -поле Amount
    -выбранное значение плеча
#### Проверка  валидации поля Limit
    1.Проверить отображение корректного значения  в поле Limit при переходе на вкладку
    2.Проверить алерт при удалении значения из поля Limit .Текст алерта "Limit price should be greater than 0"
    3.Проверить алерт при введении значения "0" в поле Limit .Текст алерта "Limit price should be greater than 0"
    4.Проверить алерт при введении значения ниже маркет прайс.Текст алерта:"The Limit price is too low. Min price 0.01"
    5.Проверить алерт при введении значения выше маркет прайс.Текст алерта:"The Limit price is above than ..."
#### Проверка  валидации поля Stop Market
    1.Проверить отображение корректного значения  в поле Stop Market при переходе на вкладку
    2.Проверить алерт при удалении значения из поля Stop Market .Текст алерта "Stop market should be greater than current market price"
    3.Проверить алерт при введении значения "0" в поле Stop Market .Текст алерта "Stop market should be greater than current market price"
    4.Проверить валидацию при создании Stop Market ордера на максимально возможную сумму при вводе в ручную .Для проверки ввести:"999999999999999" --  Алерт Отсутствует
#### Проверка  валидации поля Stop Limit
    1.Проверить отображение корректного значения  в поле Stop  при переходе на вкладку
    2.Проверить отображение корректного значения  в поле Limit  при переходе на вкладку
    2.Проверить алерт при удалении значения из поля Stop .Текст алерта: "Stop price should be greater than 0"
    3.Проверить алерт при введении значения "0" в поле Stop.Текст алерта: "Stop price should be greater than 0"
    4.Проверить алерт при вводе максимально возможного значения.Текст  алерта: "The Stop price is too high. Max price"
    5.Проверить алерт  при удалении значения в поле Limit при пустом поле Amount (Алерт отсуствует)
    6.Проверить алерт при вводе максимального значения в поле Limit при пустом  поле Amount.Текст алерта:"Your Limit price must be below your Stop price"
    7.Проверить алерт при удалении значения в поле Limit при вводе  значения в поле Amount. (Алерт отсутствует)
    6.Проверить алерт при введении значения "0" в поле Stop.Текст алерта: "Stop price should be greater than 0"
    7.Проверить алерт при вводе максимально возможного значения.Текст  алерта: "The Stop price is too high. Max price"
#### Проверка  смены колатерала
    1.Проверить возможность смены коллатерала
    2.Проверить что при смене коллатерала сохраняются значения в полях:
    -Stop, Limit, Amount, SL, TP.
    -Выбранное значение плеча.
    3.Проверить что при смене коллатерала с открытой позицией,размер плеча обновляется
#### Проверка  поля Amount
    1.Проверить что при смене  коллатерала  обновляется валидация поля Amount
    2.Проверить  граничные  значения поля Amount:
    минимальное  значение: 0.000000001
    Максимальное  значение:999999999999999
    3.Проверить алерт  при вводе миинамльно возможного значения: "Amount should be at least 0.1 TON"
    4.Проверить алерт  при вводе максимально возможного значения: "Price spread > 0.48%"
    5.Проверить что введенное в поле Amount значение,сохраняется при смене коллатерала
    6.Проверить алерт  при вводе значения превышающего баланс кошелька
    7.Проверить алерт при вводе  значения превышающего допустимый прайс импакт(решиили убрать)
    8.Проверить отображения информации о балансе на кошельке под полем Amount
    9.Проверить ввод предустановленных значений
    10.Проверить ввод  значений вручную
    11.Проверить возможность удаления введенных значений
    12.Проверить отображения плейсхолдера в поле Amount
    13.Проверить блокировку ввода невалидных символов и значений
#### Проверка  поля Leverage
    1.Проверить минимально возможное  значение  для  выбранной пары
    2.Проверить максимально возможное  значение для выбранной пары
    3.Проверить ввода значений вручную
    4.Проверить ввода  предустановленных значений
    5.Проверить отсутствия алерта  при удалении размера плеча
    6.Проверить подстановки минимально возможного значения плеча при удалении значения,после пеерстановки курсора в другое поле
    7.Проверить блокировку ввода невалидных символов и значений 
    8.Проверить автоматическую подстановку плеча на значение 10 при переходе по списку торговых пар,без открытх позиций
    9.Проверить автоматическую подстановку плеча на значение 20 для Forex пар
#### Проверка  поля Position Size
    1.Проверить значение поля Position Size при вводе значения в поле AMount
    2.Проверить значение поля Position Size при  изменении Leverage
    3.Проверить значение при отсуствии значения в поле Amount
#### Проверка  поля Entry Price 
    1.Проверить  отображение значения поля Entry price с  полем Market price
#### Проверка  поля Est. Liq. Price
    1.Проверить  корректное отображение значения поля Est. Liq. Price в зависимости от размера плеча
#### Проверка  поля Reward Points
    1.Проверить корректного отображения значения Rewards
#### Проверка  поля Spread
    1.Проверить корректное отображение значения поля Spread
#### Проверка  состояния  кнопки создания/увеличения позиции
    1.Проверить активацию кнопки содания позиции при вводе валидных значений
    2.Проверить  деактивацию кнопки содания позиции при вводе не валидных значений
#### Проверка  отображения алерта при нехватке  суммы  в TON
    1.Проверить отображение алерта при нехватке на балансе кошелька суммы в TON,необходимой для  проведения транзакции
    Текст алерта "Require 0.3075 TON balance to proceed "
#### Проверка  отображения алерта при открытии свыше 8 лимитных ордеров
    1.Проверить отображение алерта при попытке открытия 9-го лимитного ордера,под информацией о балансе кошелька
    Текст алерта : "Maximum order count reached for this pair"
#### Проверка  отображения тултипов
    1.Проверить корректное отображение тултипа  Est. Liq. Price.Текст тултипа:"Subject to change due to funding of the current position."
    2.Проверить корректное отображение тултипа  Take profit.Текст тултипа:"Please note, Take Profit settings are capped at a maximum of 300%"
#### Проверка  валидации поля Stop loss
    1.Проверить ввод предустановленных значений
    2.Проверить ввода значений вручную
    3.Проверить смену предустановленных значений при изменении размера плеча выше 30
    4.Проверить смену предустановленных значений при изменении размера плеча выше 80
    5.Проверить отображение алерта при введении значения 0 в поле ручного ввода,под информацией о балансе кошелька
    Текст алерта:"SL price can't be equal 0"
    6.Проверить отображение алерта при введении значения выще значения Маркет прайс в поле ручного ввода,под информацией о балансе кошелька
    Текст алерта:"SL price can't be greater or equal than Market Price"
    7.Проверить блокировку ввода невалидных символов и значений
#### Проверка  валидации поля Take  Profit
    1.Проверить ввод предустановленных значений
    2.Проверить ввода значений вручную
    4.Проверить отображение алерта при введении значения 0 в поле ручного ввода,под информацией о балансе кошелька
    Текст алерта:"TP price can't be equal 0"
    5.Проверить что при вводе вручную значения выше 300 %,автоматически подставляется  значение равное 300 %,после того как пользователь убрал курсор из поля ввода
    6.Проверить блокировку ввода невалидных символов и значений
#### Проверка  поля Fee
    1.Проверить корректное отображение  значения поля Fee без реф скидки
    2.Проверить корректное отображение  значения поля Fee с реф скидкой
    3.Проверить корректное отображение  значения поля Open fee для  определенной торговой пары
    4.Проверить корректное отображение значений поля Execution fee  для определенной торговой пары
    5.Проверить корректное отображение поля "Discount on commission -5% by referral code ...." при наличии реф.скидки
    6.Проверить  что скидка отображается только при введении значения в поле Amount
    7.Проверить что скидка соответствует 5 процентам
    8.Проверить что реф.скидка  выделяется зеленым цветом только после введения значения в поле Amount
    9.Проверить что при переходе по реф.ссылке на новом аккаунте,ест ь возможность смены реф.кода
    10.Проверить блокировку редактирования  реф.кода после открытия позиции
