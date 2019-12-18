# Тестовое задание на позицию Junior Android Developer

Необходимо спроектировать и разработать приложение с первоначальным вводом данных авто и водителя.

## Сценарий использования

Пользователь запускает приложение. В том случае, если первоначальный ввод не завершился (успешным вводом данных или пропуском ввода), то необходимо запустить Wizard запроса данных у пользователя.
Запрос данных делаем в 3 экрана: авто, стс, ву. Каждый из экранов можно пропустить. При попытке пропуска экрана необходимо сообщить пользователю о том, что данные авто или ву учитываться не будут и запросаить подтверждение. В случае, если пропускается ввод госномера, то ввод стс пропускается автоматически. А в случае пропуска стс, ввод госномера можно так же игнорировать.
После успешного ввода данных (или в случае запуска приложения после успешного прохождения сценария), приложение отображает данные, которые пользователь ввел ранее или констатирует факт, что они не были введены. 

## Постановка задачи

Необходимо сделать приложение, которое при запуске будет запрашивать ввод данных авто (номер и стс) и водителя (ву), далее показывать walkthrough-экраны и по итогам переходить на главный экран приложения. На главном экране приложения просто отображаем сохраненные данные и с указанием, что раздел в разработке. Пользователь так же может пропустить ввода авто и/или ву и в таком случае считаем, что он визард прошел успешно, но данные не ввел и показываем главный экран, на котором этот факт отражен.
Учесть сценарий повторного запуска после успешного ввода и пропуска (см выше).
Учесть различные форматы гос номеров: https://ru.wikipedia.org/wiki/Регистрационные_знаки_транспортных_средств_в_России а так же форматы СТС и ВУ (2 цифры, далее 2 буквы или цифры, потом 7 цифр), а так же ограничение на алфавит - могут быть исопльзованы лишь буквы, имеющие аналогичное написание в английском алфавите (например А,Е,О,Р,... и тд)
Учесть, что пользователь может осуществлять ввод на английском (например В657PO777) и такой ввод должен быть преобразован в вариант с кириллицей: В567РО777.
