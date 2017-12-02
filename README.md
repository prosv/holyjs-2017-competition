# Розыгрыш билета на HolyJS 2017 Moscow от SPB Frontend

Конкурс проводится до 4 декабря 2017 до 18:00 МСК.
Будут рассматриваться только комиты сделанные до этого времени.

## Задание
При наведении на логотип буквы должны разлетаться по экрану в случайные места, после того как они разлетелись при наведению на любую букву все буквы меняют позиции.
Через 5 секунд после последнего измения положения буквы должны собраться в изначальных позициях.

Форкайте репозиторий, присылайте Pull Request, можно творить что угодно, переписать на Ember, использовать jQuery, можно менять минификаторы, как угодно менять сборку. Но нельзя изменять index.html

Необходимо строго соблюсти все условия, победитель будет определен согласно метрикам, в случае если два участника пришлют решения с одинаковыми метриками, то победит тот, у кого последний коммит был раньше.

## Условия

- Ни на одну букву нельзя навести курсор;
- Буквы должны сохранять порядок следования слева направо;
- Буквы не должны налезать друг на друга;
- Не должны вылетать за вьюпорт;
- Внешний вид (кроме цвета) и начальные позиции букв должны остаться такими как есть;
- Буквы должны учитывать фон, на котором они находятся, на черном должны быть белыми, а на белом — черными. 
- Это условие *опционально*, не строго обязательно: если буква попадает на стык между разными фонами, буквы должны быть раскрашены частично с учетом фона;
- Должно работать в Chrome 62 без включенных флагов.

## Метрики

- В первую очередь будет учитываться размер собранных bundle.css и bundle.js файлов после команды `NODE_ENV=production yarn build`;
- Во вторую очередь при равных размерах время на layout и repaint (замер по вкладке Perfomance в Chrome Dev Tools).
