# ОПИСАНИЕ ВЕБ-СЕРВИСА

![img](https://github.com/Julia-Nemkina/qa-diploma-nemkina/blob/main/pic/img.png)

Веб-сервис предлагает купить тур по определённой цене двумя способами:

Обычная оплата по дебетовой карте.
Уникальная технология: выдача кредита по данным банковской карты.

Само приложение не обрабатывает данные по картам, а пересылает их банковским сервисам:
сервису платежей, далее Payment Gate;
кредитному сервису, далее Credit Gate.
Приложение в собственной СУБД должно сохранять информацию о том, успешно ли был совершён платёж и каким способом. Данные карт при этом сохранять не допускается.

Заявлена поддержка двух СУБД:
MySQL;
PostgreSQL.

# ИНСТРУКЦИЯ ПО ЗАПУСКУ ТЕСТИРОВАНИЯ

## Предусловия:
Установлено ПО: Git Bash, IntelliJ IDEA и Docker Desktop, DBeaver.
Дополнительно: Java 11.

## Последовательность действий:
1.  Клонировать репозиторий дипломного проекта на компьютер через команду 
"git clone https://github.com/Julia-Nemkina/qa-diploma-nemkina.git" в терминале Git Bash.
2.  Открыть скопированный проект в IntelliJ IDEA.
3. Открыть вкладку Gradle в боковой панели справа.
4. Выполнить "сборку" настроек проекта, нажав на знак со стрелочками.
5. Выбрать базу данных для запуска автотестов: 
- Открыть файл build.gradle. 
- Выбрать одну из двух баз данных, вторую "закомментировать", добавив "//" в начале строки с описанием. 
- Открыть файл application.properties. 5.4. Найти в коде выбранную базу данных, вторую "закомментировать" знаком "#" в начале строки с описанием.
6. Запустить Docker Desktop. 
7. В терминале IntelliJ IDEA запустить контейнеры командой "docker-compose up". 
8. Дождаться, пока в терминале появится информация по каждому контейнеру:
• для mysql: [Server] X Plugin ready for connections;
• для postgres: database system is ready to accept connections;
• для gate-simulator информация для тестирования:
[
{ number: '4444 4444 4444 4441', status: 'APPROVED' },
{ number: '4444 4444 4444 4442', status: 'DECLINED' }
]
9. Открыть новую вкладку в терминале IntelliJ IDEA. 
10. Запустить файл aqa-shop.jar командой:
- для mysql:
java "-Dspring.datasource.url=jdbc:mysql://localhost:3306/app" -jar aqa-shop.jar
- для postgresql:
java "-Dspring.datasource.url=jdbc:postgresql://localhost:5432/app" -jar aqa-shop.jar
11. Запустить "DBeaver" и создать подключение к mysql или postgresql (данные для подключения - порт, имя БД, пользователь, пароль - взять из файла docker-compose.yml).
12. Открыть новую вкладку в терминале IntelliJ IDEA.
13. Запустить тестирование командой:
- для mysql:
./gradlew clean test "-Ddb.url=jdbc:mysql://localhost:3306/app"
- для postgresql:
./gradlew clean test "-Ddb.url=jdbc:postgresql://localhost:5432/app"
14. Открыть новую вкладку в терминале IntelliJ IDEA. 
15. Сформировать отчёт по тестированию командой ./gradlew allureReport .
16. Завершить работу:
- остановить работу приложения командой Ctrl+C или закрыть окно терминала, в котором оно было запущено;
- остановить контейнер командой docker-compose down или командой Ctrl+C в окне терминала, в котором он был запущен.
