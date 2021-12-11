- _outline_: 2px solid tomato - для видимости блоков

- _display:inline-block_ - превращение строчных в блочные эл-ты
- _verticai-align_ - позиционирование строчных/строчно-блочных эл-ов

В body нужно задавать _margin:0_

- _margin:0 auto_ - центрирование контента

- https://cdnjs.cloudflare.com/ajax/libs/modern-normalize/1.1.0/modern-normalize.min.css

  - _порядок загрузки_: шрифты - normalize - мой css

- **_box-sizing_**:border-box - финальный размер _(включяя padding и border, но
  не margin)_

```*,
   *::before,
   *::after {
    box-sizing: border-box;
   }
```

^ это прописано в normalize - своим стилям можно не задавать

- **_Дочерние элементы (соседи)_** - это элементы с общим родителем
  - _:first-child_ _:last-child_
  - _:not(selector)_
  - _:nth-child(an+b)_
    - _a_ - период цикла (произвольное число)
    - _n_ - счётчик цикла (с нуля и увеличивается на единицу на каждой итерации)
    - _b_ - смещение (произвольное число)
    - (2n+1) = (odd) - _нечетные_
    - (2n) = (even) - _четные_
    - (n + b) - _выбирает все элементы с b и дальше_
    - (-n + b) - _выбирает первые b элементов_
    - (3n + 2) - каждый третий элемент начиная со 2-го (2, 5, 8...)
    - (2n + 4) - каждый второй элемент начиная с 4-го (4, 6, 8...)
    - (4n + 5) - каждый четвёртый элемент начиная с 5-го (5, 9, 13...)
  - _:nth-last-child(an+b)_ - аналог :nth-child() но отсчёт ведётся с конца
