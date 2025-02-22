# NIT Test Download an Run PoC

NIT Test Download and Run Proof of Concept - это попытка систематизировать техники Download and Execute, написанные на языку Visual C++ (конкеретно для Visual Studio 2017), для реализации различных целей (например, для доставки и установки на компьютер программ, текстовых файлов и т.п.).

Данный набор функций:

- Определяет текущую версию операционной системы.
- Программно определяет местоположение основынх папок для продуктов New Internet Technologies, личные папки пользователя Microsoft Windows, и позволяет загружать в них файлы из Интернете по протоколу http и https.
- Позволяет запускать на исполнение документы с зарезервированными в Microsoft Windows расширениями, Windows Script, Windows Shell, Powershell 5.1, исполняемые файлы из командной строки. В дальнейшем несложно написать программу для скрытой установки файлов из дистрибутивов.

Как и вся указанная выше технология, созданные в рамках этого PoC файлы могут (но не обязательно) детектироваться антивирусом как файлы, содержащее различное malware. Об этом надо предупреждать пользователей при коммерческом распространении прграмм, созданных на основе этого PoC. Кроме того, этот концепт может сам использоваться для доставки вредоносной нагрузки, хотя это запрещено лицензией.

## Установка

Данная программа не требует установки и готова к запуску сразу после компиляции.

При своей работе программа выводит информацию о своей работе и о возникающих ошибках.

### Модификация

Классы программы поставляются "как есть", их модификация, как правило, не требуется (только для исправления ошибок и привнесения новых функций).

Основная логика программы реализована в файлах `NIT.Test.Procedure.000.cpp` и `NIT.Test.Procedure.000.h`. Именно их нужно менять при кастомизации программы и приспособлении её под собственный функционал.

## Лицензия

Программа распространяется под лицензией GPLv3.

Программа написана в образовательных целях. Запрещено использовать программу для доставки любого вредоносного содержимого.