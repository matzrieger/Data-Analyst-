## Для кредитного отдела банка необходимо установить влияние семейного положения и количество детей клиента на факт погашения кредита. Данный анализ поможет в создании скоринга для предугадывания последующих запросов на кредитование
### Предобработка
- Поиск и замена нулевых значений на медианное, дабы не испортить выборку
- Составление баг-репорта 
- Замена типа данных, смена регистра имен столбцов, поиск и удаление дубликатов
### Лемматизация
- Преобразование данных лемматизируемого столбца
- Использование библиотеки pymystem3 для выделения лемм текста
- Обозначение вида кредита. 
### Категоризация данных 
Создание функции для оценки заемщиков по количеству детей, семейному положению, уровню дохода и цели кредита
### Вывод
В результате работы над проектом выяснил, что бездетные семьи имеют меньшую кредитную нагрузку, женатые чаще холостых возвращают кредиты в срок, не важно какой уровень дохода у клиентов - это не зависит на возврат кредита, а кредиты на свадьбу или операции с недвижимостью будут выплачены быстрее остальных. Предлагаю использовать эти парамметры для кредитного скоринга, что позволит автоматизировать работу с заемщиками, а также увеличит скорость по выносу решения о предоставления кредита
