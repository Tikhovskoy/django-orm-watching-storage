# Пульт охраны банка

Это внутренний репозиторий для сотрудников банка «Сияние». Если вы попали в этот репозиторий случайно, то вы не сможете его запустить, т.к. у вас нет доступа к БД, но можете свободно использовать код вёрстки или посмотреть, как реализованы запросы к БД.

Пульт охраны — это сайт, который можно подключить к удалённой базе данных с визитами и карточками пропуска сотрудников нашего банка.

---

### Функционал
- Просмотр активных пропусков сотрудников банка.
- Учет посещений хранилища и анализ времени пребывания.
- Вывод подробной информации о каждом визите.
- Логирование всех посещений.

## Как установить

1. **Клонируйте репозиторий**:
   ```bash
   git clone https://github.com/ваш-репозиторий/django-orm-watching-storage.git
   cd django-orm-watching-storage
   ```

2. **Создайте и активируйте виртуальное окружение**:
   ```bash
   python -m venv venv
   source venv/bin/activate  # Для Linux/MacOS
   venv\Scripts\activate  # Для Windows
   ```

3. **Установите зависимости**:
   ```bash
   pip install -r requirements.txt
   ```

4. Скопируйте файл `.env.example` и переименуйте его в `.env`.:
   ```env
	ALLOWED_HOSTS=127.0.0.1,localhost,yourdomain.com
	DEBUG=False  # Или False
	DB_ENGINE=django.db.backends.postgresql
	DB_HOST=your_database_host
	DB_PORT=your_database_port
	DB_NAME=your_database_name
	DB_USER=your_database_user
	DB_PASSWORD=your_database_password
	SECRET_KEY=your_secret_key
   ```

5. **Запустите сервер**:
   ```bash
   python manage.py runserver 0.0.0.0:8000
   ```

После запуска сервер будет доступен по адресу [http://127.0.0.1:8000](http://127.0.0.1:8000).

---

## Как использовать

- На главной странице вы увидите список активных пропусков.
- Вы можете зайти на страницу информации о конкретном пропуске.
- Можно просмотреть список сотрудников, находящихся в хранилище.

---

## Лицензия
Этот проект предназначен для внутреннего использования и не должен распространяться без разрешения владельцев.

