Массовое добавление сотрудников списком в домен Active Directory.

Чтобы воспользоваться программой достаточно перейти на сайт - https://tkachukds.github.io/AD-User-Importer/

Инструкция:
1. Вносим данные вашего домена в AD "A3f.local", "BB.ru"
   
![image](https://github.com/tkachukds/AD-User-Importer/assets/103854079/42c38fea-4fb5-49a1-86ef-44ac91fba990)

2. Можно изменить стандартный пароль от всех пользователей. ВНИМАНИЕ: Как только пользователь войдет, он будет обязан сменить пароль. Поэтому ставить сложный пароль просто нет смысла.

![image](https://github.com/tkachukds/AD-User-Importer/assets/103854079/34b29db5-eb6f-4f05-8d03-2c5a7dcefcff)

 3. Вносим OU
    
![image](https://github.com/tkachukds/AD-User-Importer/assets/103854079/c78bb74d-3180-4516-a0b6-478936a150be)

OU можно посмотреть в папке с пользователями в AD

4. Вносим список пользователей, которых нужно добавить
   
 ![image](https://github.com/tkachukds/AD-User-Importer/assets/103854079/7987d884-fd9c-43c9-9472-aad97e6434ca)

и нажимаем СОЗДАТЬ

Появится код (можно проверить все ли правильно) а также создается файл  addusers.ps1
![image](https://github.com/tkachukds/AD-User-Importer/assets/103854079/0f05bd5f-a317-4e2f-ac63-8c0a8f7cdc9b)
![image](https://github.com/tkachukds/AD-User-Importer/assets/103854079/999e1c4d-528d-478d-995c-1ea956aa6bb0)


Запускаем файл addusers.ps1 на Windows Server и пользователи будут автоматически созданы.


Логин формируется автоматически по алгоритму - ТРАНСЛИТ"первая буква имени.фамилия полностью"

Если что-то пойдет не так, PowerShell об этом вам сообщит. (например: если такой пользователь уже есть)

С ув. Ткачук Денис.
