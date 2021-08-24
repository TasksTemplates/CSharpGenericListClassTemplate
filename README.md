Общая информация
В этой задаче требуется реализоват двусвязный список из первой части задачи в виде отдельного класса.
Задача
1.	Реализуйте двусвязный список в виде класса с заданным набором методов (см. раздел “Реализация”).
2.	Напишите тестовую программу

Реализация:
```cs  
class LinkedList<T> 
{
    public LinkedList();
    public LinkedList(LinkedList other);

    //Возвращает первый элемент списка.
    public T Front();
    //Возвращает последний элемент списка.
    public T Back();
    //Возвращает истину, если значение value содержится в списке.
    public bool Contains(T value);
    //Возвращает количество вхождений значения value в список.
    public int Count(T value);
    //Возвращает размер списка.
    public int Size();
    //Возвращает истину, если список пуст.
    public bool Empty();
    //Удаляет элемент c номером position.
    public void Erase(uint posisition);
    //Удаляет элементы в интервале [begin, end).
    public void Erase(uint begin, uint end);
    //Очищает список.
    public void Clear();
    //Удаляет все вхождения value в список.
    public void Remove(T value);
    //Удаляет последний элемент списка.
    public T PopBack();
    //Удаляет первый элемент списка.
    public T PopFront();
    //Добавляет значение value в конец списка.
    public void PushBack(T value);
    //Добавляет значение value в начало списка.
    public void PushFront(T value);
    //Вставляет значение value перед элементом, на который указывает before
    public void Insert(uint position, T value);
}
```

Так же перегрузить метод Equals, позволяющий сравнить два списка. Внутри списка ещё реализовать свойство длинны списка, доступное только для чтения для классов вне списка.
