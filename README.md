[![Build status](https://ci.appveyor.com/api/projects/status/s14o1ke1a9e1g3o7/branch/main?svg=true)](https://ci.appveyor.com/project/marinaustinovich/ahj-homeworks-env/branch/main)

deployment: https://marinaustinovich.github.io/ahj-homeworks-env/

### 1. Yarn

#### Легенда

Вы работаете с новой командой, в которой в качестве пакетного менеджера используется `yarn`. От верстальщика вам пришёл небольшой макет, для которого необходимо собрать инфраструктуру на базе Webpack, ESLint, Babel, Jest, Webpack Dev Server.

Картинка, указанная в `index.html` в итоговой сборке, без необходимости явного её импорта в `index.js`. Кроме того, иконка `favicon.ico` тоже  в дистрибутиве.

[Исходники к задаче](https://github.com/netology-code/ahj-homeworks/tree/master/yarn-cd).

**Важно: эта задача не предполагает развёртывания в AppVeyor и GitHub Pages.**

---

### 2. Continuous Deployment

#### Легенда

Разворачивание настроенного проекта из задачи №1 в связке из AppVeyor и GitHub Pages.

#### Описание


Проект настроен так, чтобы без тестов код завершения был 0 — команда `yarn test` проходила без ошибки.

---

### 3. Разделение конфигураций (задача со звёздочкой)

#### Легенда

На данный момент одна конфигурация Webpack: для разработки и для production. В больших проектах конфигурации чаще всего разделяют в том числе потому, что для production применяются плагины оптимизации, выполнение которых может занять достаточно длительное время.

#### Описание

Конфигурация разделена на три части:
* общая;
* prod — здесь указано только `mode: 'production'` и настройки оптимизации для плагинов Terser и OptimizeCSSAssets;
* dev.

