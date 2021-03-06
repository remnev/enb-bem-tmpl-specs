История изменений
=================

0.11.2
------

### Исправления ошибок

* Исправлено подключение дополнительных уровней для теста ([#87]).

0.11.1
------

### Исправления ошибок

* Исправлено сохранение актуальных HTML файлов ([#85]).
* Исправлена ошибка, из-за которой не запускались тесты для эталонов с пустыми файлами ([#83]).

### Зависимости

* Модуль `enb-bem-i18n@0.2.1` обновлён до версии `0.3.0`.
* Модуль `html-differ@1.3.0` обновлён до версии `1.3.1`: улучшено отображение различий.
* Модуль `istanbul@0.3.7` обновлён до версии `0.3.14`.
* Модуль `jade@1.9.2` обновлён до версии `1.10.0`.
* Модуль `js-beautify@1.5.4` обновлён до версии `1.5.5`: улучшено форматирование HTML.
* Модуль `lodash@3.5.0` обновлён до версии `3.9.3`.
* Модуль `minimatch@2.0.3` обновлён до версии `2.0.8`.
* Модуль `mocha@2.2.1` обновлён до версии `2.2.5`.
* Модуль `vow@0.4.8` обновлён до версии `0.4.9`.

### Остальное

* Теперь будет выводиться предупреждение, если для эталоне не хватает одного из файлов: HTML или BEMJSON ([#83]).

0.11.0
------

### Крупные изменения

Добавлена поддержка коментариев `/ istanbul ignore next */` для игнорирования участков кода при подсчёте покрытия тестами ([#73]).

### Исправления ошибок

* Исправлена ошибка, из-за которой не переопределялись эталоны ([#74]).

### Остальное

* Модуль `js-beautify@1.5.4` обновлён до версии `1.5.5`: улучшено форматирование HTML [beautify-web/js-beautify#524](https://github.com/beautify-web/js-beautify/issues/524).
* Модуль `enb-bem-techs@1.0.3` обновлён до версии `1.0.4`.
* Модуль `istanbul@0.3.6` обновлён до версии `0.3.7`.
* Модуль `lodash@3.3.0` обновлён до версии `3.5.0`.
* Модуль `minimatch@2.0.1` обновлён до версии `2.0.3`.
* Модуль `mocha@2.1.0` обновлён до версии `2.2.1`.

0.10.0
------

* Добавлена опция `htmlDiffer`: позволяет переопределять настройки для сравнения HTML ([#54]).
* Модуль `html-differ@1.1.0` обновлён до версии `1.3.0`: Исправлена ошибка при обработке [масок](https://github.com/bem/html-differ/blob/master/README.ru.md#Маски) в HTML.
* Модуль `lodash@3.2.0` обновлён до версии `3.3.0`.

0.9.0
-----

* Модуль `html-differ@1.0.8` обновлён до версии `1.1.0`: добавлена поддержка [масок](https://github.com/bem/html-differ/blob/master/README.ru.md#Маски) в HTML.

0.8.0
-----

* Добавлена возможность задавать дополнительный уровень переопределения для теста ([#70]).
* Исправлена ошибка, из-за которой тесты блока запускались в тестах его элементов и модификаторов ([#68]).
* Модуль `istanbul@0.3.5` обновлён до версии `0.3.6`.

0.7.0
-----

### Крупные изменения

* Добавлена поддержка асинхронных шаблонизаторов (@zxqfox [#41]).
* Добавлена [возможность фильтровать](https://github.com/enb-bem/enb-bem-tmpl-specs#Фильтрация-тестов) запускаемые тесты с помощью опции `grep` или переменной окружения `BEM_TMPL_SPECS_GREP` (@zxqfox [#61]).

### Исправления ошибок

* Исправлена ошибка, из-за которой добавлялся код, имитирующий `BEM.I18N`, при `langs: false`.
* Исправлена ошибка сборки шаблонизаторов с учётом локализации при `coverage: false`.
* Исправлена ошибка, из-за которой не запускалась сборка шаблонизаторов, необходимых для выполнения тестов, если целью сборки был только таргет `?.tmpl-spec.js`.
* Исправлено кэширование для сборки таргета `?.tmpl-spec.js`: пересборка будет происходить только по необходимости.

### Остальное

* Модуль `lodash@3.1.0` обновлён до версии `3.2.0`.

0.6.4
-----

* Модуль `html-differ@1.0.7` обновлён до версии `1.0.8`: теперь только условные коментарии учитываются при сравнении `html`.
* Модуль `jade@1.9.1` обновлён до версии `1.9.2`.

0.6.3
-----

* Исправлена имитация `BEM.I18M`: добавлена поддержка `param` ([#52]).
* Исправлена ошибка из-за которой не подключалась имитация `BEM.I18M` при выключенном `coverage` ([#50]).
* Модуль `lodash@3.0.1` обновлён до версии `3.1.0`.

0.6.2
-----

* Шаблонизация BEMJSON-эталонов теперь происходит независимо от выполнения предыдущих запусков ([#49]).
* Исправлена ошибка, когда нет эталонов и папка `tmpl-specs` пуста ([#47]).
* Модуль `html-differ@1.0.5` обновлён до версии `1.0.7`: коментарии теперь учитываются при сравнении `html`.
* Модуль `bem-naming@0.5.0` обновлён до версии `0.5.1`.
* Модуль `enb-bem-i18n@0.1.2` обновлён до версии `0.2.1`.
* Модуль `enb-bem-techs@1.0.0` обновлён до версии `1.0.3`.
* Модуль `jade@1.8.2` обновлён до версии `1.9.1`.
* Модуль `lodash@2.4.1` обновлён до версии `3.0.1`.
* Модуль `mocha@2.0.1` обновлён до версии `2.1.0`.
* Модуль `vow@0.4.7` обновлён до версии `0.4.8`.
* Модуль `vow-fs@0.3.3` обновлён до версии `0.3.4`.

0.6.1
-----

* Исправлена сборка `BEM.I18N` для опции `langs` со значением `true`.
* Модуль `enb-bem-pseudo-levels` обновлён до версии `0.2.6`.
* Модуль `html-differ` обновлён до версии `1.0.5`.
* Модуль `bem-naming` обновлён до версии `0.5.0`.

0.6.0
-----

* Добавлена опция `langs` (#12).
* Исправлены ошибки при использовании в Windows ([#39]).
* Модуль `enb-source-map` обновлён до версии `1.5.0`.
* Модуль `jade` обновлён до версии `1.8.2`.

0.5.2
-----

* Модуль `enb-bem-techs` обновлён до версии `1.0.0`.
* Модуль `enb-bem-pseudo-levels` обновлён до версии `0.2.5`.
* Модуль `istanbul` обновлён до версии `0.3.5`.

0.5.1
-----

* Исправлен запуск тестов для `pre` режима magic-нод.
* Модуль `jade` обновлён до версии `1.8.0`.
* Модуль `mocha` обновлён до версии `2.0.1`.

0.5.0
-----

* Добавлена возможность подсчёта покрытия кода тестами ([#36]).
* Модуль `bem-naming` обновлён до версии `0.4.0`.
* Модуль `enb-bem-techs` обновлён до версии `1.0.0-rc`.

0.4.1
-----

* Исправлен `html` и `summary` отчёты ([#31]).
* Модуль `mocha` обновлён до версии `2.0.1`.
* Модуль `vow` обновлён до версии `0.4.7`.

0.4.0
-----

* Переход на `enb-magic-factory@0.3.x`.
* Модуль `mocha` обновлён до версии `2.0.0`.

0.3.1
-----

* Улучшена сборка `?.tmpl-specs.js` таргета.
* Улучшен `html` отчёт.
* Опцию `saveHtml` теперь можно задавать через переменную окружения `BEM_TMPL_SPECS_SAVE_HTML`.
* Исправлено кэширование для опции `saveHtml`.
* Исправлена сборка по `depsByTech` (#16).
* Для форматирования html теперь используется `js-beautify` пакет, вместо `html`.

0.3.0
-----

* Добавлены `summary` и `html` отчёты.

[#83]: https://github.com/enb-bem/enb-bem-tmpl-specs/issues/83
[#74]: https://github.com/enb-bem/enb-bem-tmpl-specs/issues/74
[#73]: https://github.com/enb-bem/enb-bem-tmpl-specs/issues/73
[#70]: https://github.com/enb-bem/enb-bem-tmpl-specs/issues/70
[#68]: https://github.com/enb-bem/enb-bem-tmpl-specs/issues/68
[#61]: https://github.com/enb-bem/enb-bem-tmpl-specs/issues/61
[#54]: https://github.com/enb-bem/enb-bem-tmpl-specs/issues/54
[#50]: https://github.com/enb-bem/enb-bem-tmpl-specs/issues/50
[#47]: https://github.com/enb-bem/enb-bem-tmpl-specs/issues/47
[#41]: https://github.com/enb-bem/enb-bem-tmpl-specs/issues/41
[#87]: https://github.com/enb-bem/enb-bem-tmpl-specs/pull/87
[#85]: https://github.com/enb-bem/enb-bem-tmpl-specs/pull/85
[#52]: https://github.com/enb-bem/enb-bem-tmpl-specs/pull/52
[#49]: https://github.com/enb-bem/enb-bem-tmpl-specs/pull/49
[#39]: https://github.com/enb-bem/enb-bem-tmpl-specs/pull/39
[#36]: https://github.com/enb-bem/enb-bem-tmpl-specs/pull/36
[#31]: https://github.com/enb-bem/enb-bem-tmpl-specs/pull/31
