# css-grid

.grid-container {

    display: grid; представлен в виде сетки или же таблицы
    grid-template-columns: repeat(3, minmax(150px, 300px)); 
    /* свойство repeat для повторных действий, 
    grid-template-columns определяет имена линий и размеры грид-колонок. */
    
    grid-template-rows: repeat(3, minmax(100px, auto)); 
    /* определяет имена линий и размеры полос грид-рядов */
    
    /* fr единица измерения в гридах для колонок */
    
    /* grid-template-rows: repeat(3, minmax(100px, auto)); 
    свойство minmax регулирует максимальное и минимальное разрешение */ 
    
    /* grid-template-columns: [col1-s] 150px [col2-s] 150px [col3-s] 150px; */
    /* grid-template-rows: [row1-s] 150px [row2-s] 150px [row3-s] 150px [row4-s]; */
    
    grid-auto-rows: minmax(100px, auto); 
    /* определяет размер неявно созданной дорожки строки сетки или шаблона */
    
    /* grid-auto-columns: 200px; 
    определяет размер неявно созданной дорожки столбца сетки или шаблона */
    
    /* column-gap: 10px; 
    задаёт отступ между колонками */
    
    /* row-gap: 10px; 
    задаёт отступ между рядами */
    
    gap: 10px; 
    /* комбинированное свойство отступов между колонками и рядами*/
    
    grid-auto-flow: row; 
    /* свойство задает либо колоночный, либо строчный вид для элементов */
    
    /* minmax ( , ) 
    свойство задает минимальное и максимальное разрешение колонкам */
    
    /* auto-fill 
    ЗАПОЛНЯЕТ строку таким количеством столбцов, сколько может вместиться */
    
    /* auto-fit 
    ВПИШЕТ ДОСТУПНЫЕ В ТЕКУЩИЙ МОМЕНТ столбцы в пространство, чтобы они заняли все доступное место */
    
    /* align-items: center; 
    свойство align-items выравнивает все элементы текущей линии */
    
    /* justify-items: center; 
    свойство justify-items выравнивает все элементы вдоль соответствующей оси */
    
    /* justify-content: space-around; 
    распределяет пространство между и вокруг элементов контента вдоль главной оси */
    
    /* align-content: center; 
    устанавливает распределение пространства между и вокруг элементами контента, 
    [вертикально] 
    нагляднее всего работает с назначенной высотой */
    
    place-content: center space-around;
    /* place-content: justify-content + align-content; */
    /* place-items: center center; */
    /* place-items: justify-items + align-items; */
    
}

.grid-elem {

    background-color: rgba(1, 1, 96, 1);
    color: #fff;
    line-height: 50px;
    text-align: center;
    font-size: 26px;
    border: 1px solid #000;
    border-radius: 4px;
    
}

#first {

    /* grid-column: col1-s/col3-s; 
    свойство назначает grid-столбцы элементу по их именам */
    
    /* grid-column-start: 1; 
    свойство определяет начало элемента в колоночной сетке */
    
    /* grid-column-end: 3; 
    свойство определяет где заканчивается элемент в колоночной сетке */
    
    /* grid-column: 1 / 3; 
    комбинированное свойство для колоночных сеток */
    
    /* align-self: center; 
    выравнивает элемент по текущей линии, переопределяя значение свойства align-items */
    
    /* justify-self: end; 
    выравнивает элемент вдоль соответствующей оси */
    /* p.s общее свойство можно перебивать если назначить свойство определенному элементу */
    /* пример: */
    /* justify-self: end; элемент будет вываливаться в доступный конец колонки */
    
    /* place-self: */
    /* place-self: justify-self + align-self; */
}

#second {

    /* grid-row-start: 3; 
    свойство определяет начало элемента в строчной сетке */
    
    /* grid-row-end: 4; 
    свойство определяет где заканчивается элемент в строчной сетке */
    
    /* grid-row: 3 / 4; 
    комбинированное свойство для строчных сеток */
    
    /* grid-column: 2; */ 
    комбинированное свойство для колоночных сеток 
    
    /* grid-row: row3-s; 
    свойство назначает элементу grid-ряды по их именам */
    /* grid-column: col2-s; */ 
}

#third {

    /* grid-row: row2-s/row4-s; */
    /* grid-column: col3-s; */
    
}
