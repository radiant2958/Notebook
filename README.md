# Notebook

Этот код реализует простой текстовый редактор, используя шаблон проектирования Model-View-Presenter (MVP). Он позволяет пользователю добавлять, удалять и печатать записи в блокноте, который сохраняется в файл.

Класс Model хранит данные блокнота и управляет вводом/выводом файла. Интерфейс FileHandler и класс FileHandlerClass реализуют сохранение и загрузку данных блокнота из файла. Классы Notebook и Record определяют структуры данных для заметок.

Класс Presenter выступает в роли посредника между Model и View. Он получает ввод от пользователя через View и соответствующим образом изменяет Model.

Интерфейс View и класс ConsoleView реализуют пользовательский интерфейс. Класс ConsoleView позволяет пользователю вводить текст через консоль и отображать данные блокнота.

Интерфейс Command и его реализации, AddRecord, RemoveRecord и PrintNotebook, представляют действия, которые может выполнить Presenter.
