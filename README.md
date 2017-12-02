# Задание traf_excercise

Целью задания является анализ информации о трафике прошедшим через некое сетевое устройство, с целью вычисления необходимой аналитический информации. Все хосты-участники считаются наблюдаемым сегментом сети.

## Данные

Информация находятся в файле traf.txt. Каждая строка содержит одну запись о переданных данных между двумя узлами наблюдаемого сегмента сети. Поля в строке отделены символом ';'.

### Поля данных (по порядку слева-направо)

- IP:Port хоста с которого отправлены данные
- MAC хоста с которого отправлены данные
- IP:Port хоста на который отправлены данные
- MAC хоста на который отправлены данные
- Признак UDP: 'true' - UDP, 'false' - TCP
- Размер переданных данных, байт
- Время передачи, миллисекунд

## Задание

Проанализируйте информацию в файле и ответьте на следующие вопросы в отношении наблюдаемого сегмента сети:

- Сколько уникальных узлов в наблюдаемой сети (штук)?
- Какова средняя скорости передачи данных всей наблюдаемой сети (байт/сек)?
- Основываясь на данных о трафике, верно-ли утверждение "UDP используется для передачи данных с максимальной скоростью"?
- Укажите 10 самых активных узлов сети по критерию количества сессий передачи данных (штук)
- Укажите 10 узлов сети с самой высокой скоростью передачи данных (байт/сек)
- Есть-ли в сети узлы, которые могут являться посредниками (т.н. PROXY) между другими узлами? Укажите их, если они есть

## Результат выполнения задания

Результат должен содержать следующие артефакты:

- Ответы на вопросы задания
- Исходный код, который был создан для выполнения задания
- Инструкция по запуску исходного кода + перечень необходимых программных компонент для его запуска

## Требования к выполнению задания

- Реализация должна быть выполнена на платформе Linux
- Можно использовать любые программные инструменты разработки (языки, библиотеки, IDE и т.п.)
- Нельзя использовать готовое ПО для анализа данных, т.е. все расчеты должны быть выполнены самописным кодом
