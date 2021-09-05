# os226-2020

## Как сдавать

Задания предлагается сдавать в виде Pull Requestов.

Язык общения в PR/issues: русский

На каждый PR запускается набор тестов.

Если тесты успешно проходят и в коде нет криминала, PR получает метку "accepted" и закрываются.
PR с меткой accepted учитываются на зачёте в положительную сторону.

Если тесты не проходят, то PR получает метку "issues".

Чтобы проверить тесты локально (до коммита/пуша/создания PR), достаточно запустить `test/run.sh`.
Например:
```
os226-2020$ ./test/run.sh ; echo $?
```
echo выводит код возврата, он должен быть нулём.

Если тесты прошли, но в коде есть грубые ошибки, то PR получает метку "issues".
Пример грубой ошибки: модификация тествой системы, чтобы она засчитывала неверные решения :-)

Для того, чтобы изменить уже посланое решение, достаточно сделать push в ваш бранч.
PR автоматически обновится и перетестируется.

## Метки
* accepted - решение засчитано, PR закрывается.
* issue - решение не засчитано, есть существенные замечания. Замечания можно исправлять до таймаута замечания.
* partial - решение зачитано частично, есть замечания. Замечания можно исправлять. Закрытый PR в таком состоянии стоит 1/2 балла.

PR с метками висит до исправления или конца следующей недели, затем закрывается.
