<h1>
Inheritance in JavaScript
</h1>

<div>
Каждый объект в js имеет прототип. Связь(доступ) к этому прототипу осуществляется в объекте через скрытое свойство [[Prototype]].
Прототипом будет или объект (на основе которого создан объект) или null если вверх по цепочке таких объектов не осталось.

__proto__ - это ссылка на скрытое свойство объекта [[Prototype]]. Тоесть обратится к [[Prototype]] возможно через свойство __proto__
Все объекты имеют __proto__. При стандартном переборе свойств оно не отображается, однако его значение можно вызвать напрямую или увидеть в консоле.
</div>

<br/>

<div>
Для того чтобы проверить является ли свойство объекта унаследованным или оно определено
в самом объекте существует метод объекта: <code>hasOwnProperty()</code>
</div>

<br/>

<div>
У всех объектов есть свойство Constructor (<code>let test = {}; test.constructor</code>), ссылка на функцию, которая выступила конструктором.
</div>

<br/>

<div>
Конструктором в js называется функция, создающая объект. В случае отсутствия инициализирующих параметров в конструкторе, скобки можно опускать (let test = new Parent).
У Конструктора, тоесть у функции, есть свойство prototype (let ttt = function(){}; у стрелочных не так!). В это свойство можно передать объект, который станет прототипом для экземпляров Конструктора.
</div>

<br/>

<div>
<a href="https://codepen.io/paawel/pen/XZpmdJ?editors=0012">Quick sample</a>
</div>


Тонкий клиент (Thin client) - переносит задачи по обработке информации на сервер
Толстый клиент (Rich client) - производит обработку информации на клиенте, независимо от сервера. При архитектуре Толстого клиента сервер может являться просто хранилищем данных.
При всех плюсах архитектуры Толстого клиента следует все же помнить, что javascript в браузере можно отключить.
