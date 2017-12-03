# Задание traf_excercise

Целью задания является разработка ПО для анализа информации о трафике, прошедшим через некое сетевое устройство. Все хосты-участники считаются наблюдаемым сегментом сети.

## Данные

Информация находятся в файле traf.txt. Каждая строка содержит одну запись о переданных данных между двумя узлами наблюдаемого сегмента сети. Поля в строке отделены символом ';'.

### Поля данных (по порядку в строке, слева-направо)

- IP:Port хоста с которого отправлены данные
- MAC хоста с которого отправлены данные
- IP:Port хоста на который отправлены данные
- MAC хоста на который отправлены данные
- Признак UDP: 'true' - UDP, 'false' - TCP
- Размер переданных данных, байт
- Время передачи, миллисекунд

## Задание

Разработайте ПО котрое проанализирует информацию в файле и ответит на следующие вопросы, в отношении наблюдаемого сегмента сети:

- Сколько уникальных узлов в наблюдаемой сети (штук)?
- Какова средняя скорости передачи данных всей наблюдаемой сети (байт/сек)?
- Основываясь на данных о трафике, верно-ли утверждение "UDP используется для передачи данных с максимальной скоростью"?
- Укажите 10 узлов сети с самой высокой скоростью передачи данных (байт/сек).
- Укажите 10 самых активных подсетей /24 по критерию количества сессий передачи данных (штук).
- Есть-ли в сети узлы, которые могут являться посредниками (т.н. PROXY) между другими узлами? Укажите их, если они есть.

Записи с некорректными данными нужно не учитывать в расчетах.

## Требования к выполнению задания

- Реализация должна быть выполнена на платформе Linux
- Можно использовать любые программные инструменты разработки (языки, библиотеки, IDE и т.п.)
- Нельзя использовать готовое ПО для анализа данных, т.е. все расчеты должны быть выполнены самописным кодом

## Результат выполнения задания, в случае неинтерактивного интервью

Результат должен содержать следующие артефакты:

- Исходный код, который был создан для выполнения задания и дающий ответ на вопросы задания, путем вывода на экран
- Инструкция по запуску исходного кода + перечень необходимых программных компонент для его запуска
