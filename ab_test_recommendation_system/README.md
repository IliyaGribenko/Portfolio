# A/B тест рекомендательной системы
## Цели и описание проекта

В компании проводится тестирование изменений, связанных с внедрение улучшенной рекомендательной системы.

Задача — провести оценку результатов A/B-теста. А именно:
- оценить корректность проведения теста
- проанализировать результат теста

В нашем распоряжении есть датасет с действиями пользователей, техническое задание и несколько вспомогательных датасетов.

**Техническое задание**

- название теста: `recommender_system_test`;
- группы: А - контрольная, B - новая платежная воронка;
- дата запуска: 2020-12-07
- дата остановки набора новых пользователей: 2020-12-21;
- дата остановки: 2021-01-04;
- аудитория: 15% новых пользователей из региона EU;
- назначение теста: тестирование изменений, связанных с внедрением улучшенной рекомендательной системы;
- ожидаемое количество участников теста: 6000
- ожидаемый эффeкт за 14 дней с момента регистрации:
    - пользователи покажут улучшение каждой метрики не менее, чем на 10%
        - конверсии в просмотр карточек товаров - событие `product_page`
        - просмотр корзины - `product_cart`
        - покупки - `purchase`

## Инструменты

- python
- datetime
- pandas
- matplotlib
- seaborn
- plotly
- statsmodels

 ## Общие выводы
 
 Найден ряд ошибок допущенных при проведении теста.
 - практически все пункты `тз` не выполняются
 - контрольная и тестовая группы сформированы не случайным образом
    - A/A тест не проводился
 - не контролируются значения метрик, которые могут быть случайно ухудшены
 - не достигнут ожидаемый эффект улучшения метрик
 
 В связи с вышеперечисленными ошибками при проведении теста его результатам доверять не стоит.
