# goit-algo-hw-04
# Порівняння алгоритмів сортування: злиттям, вставками та Timsort

## Опис завдання
Дана робота полягає в порівнянні ефективності трьох алгоритмів сортування: сортування злиттям, сортування вставками та алгоритм Timsort, який використовується у вбудованих функціях сортування sorted та sort мови програмування Python. Ефективність буде оцінена за часом виконання алгоритмів на різних наборах даних. Для вимірювання часу виконання алгоритмів використовувався модуль timeit.


Для порівняння алгоритмів сортування були використані набори даних різного розміру. Результати тестування наведені в таблиці:

| Алгоритм/розмір | 100 | 500 | 1000 |
| --- | --- | --- | --- |
| Merge Sort | 0.0388 | 0.2577 | 0.5122 |
| Insertion Sort | 0.0511 | 1.1132 | 4.3155 |
| _Timsort_ | _0.0093_ | _0.0604_ | _0.1170_ |


### Сортування через злиття (Merge Sort)
Сортування через злиття виконується за часовою складністю $O(n∙logn)$, що означає, що при збільшенні розміру вхідного масиву час виконання збільшується логарифмічно. Цей алгоритм ефективно сортує навіть великі масиви даних.

### Сортування вставками (Insertion Sort)
Сортування вставками має часову складність $O(n^2)$. Хоча воно є ефективним для невеликих наборів даних, на великих масивах його продуктивність зменшується через квадратичну залежність від розміру вхідних даних.

### Timsort
Timsort використовує комбінацію методів сортування злиттям і вставками. Цей алгоритм демонструє кращу часову ефективність у порівнянні з іншими алгоритмами сортування. На відміну від окремих алгоритмів злиття та вставок, Timsort у великій мірі оптимізований для різних типів вхідних даних, що робить його набагато більш універсальним і продуктивним.

## Висновки
З урахуванням наданих даних порівняння, алгоритм Timsort виявився набагато ефективнішим у порівнянні з Merge Sort та Insertion Sort для різних розмірів вхідних наборів даних.
