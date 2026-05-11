# Лабораторная работа №6

## Разработка мобильного приложения на Swift

### Цель работы

Изучить основы разработки мобильных приложений на языке Swift в среде Xcode, научиться работать с элементами пользовательского интерфейса, системой контроля версий Git и сервисом GitHub.

---

# Ход выполнения работы

## Шаг 1. Создание папок проекта

На операционной системе Windows была создана структура каталогов для лабораторной работы с использованием Git Bash.

Использованные команды:

```bash id="e88qlc"
mkdir labtp2025
cd labtp2025
mkdir labrabota6
cd labrabota6
mkdir lab6task1
cd lab6task1
```

### Скриншот

<img width="684" height="536" alt="1_создание_папок" src="https://github.com/user-attachments/assets/d1d9641e-a6e5-4042-91db-767048488f14" />


---

## Шаг 2. Создание репозитория GitHub

Был создан репозиторий для лабораторной работы через GitHub Classroom.

### Скриншот

<img width="1324" height="598" alt="2_accept_repo" src="https://github.com/user-attachments/assets/c42ba36a-50b8-4eaf-97e3-c37977318625" />


---

## Шаг 3. Проверка созданного репозитория

После принятия задания был создан личный репозиторий GitHub.

### Скриншот

Вставить скрин:

<img width="682" height="718" alt="3" src="https://github.com/user-attachments/assets/15d13706-2b91-4bc7-a8a1-6ad75680bb04" />


---

## Шаг 4. Инициализация Git репозитория

В локальной папке проекта был инициализирован Git репозиторий.

Использованные команды:

```bash id="zjl1zj"
git init
git add README.md
git commit -m "first commit"
```

### Скриншот

<img width="496" height="224" alt="4_feature_branch png" src="https://github.com/user-attachments/assets/ae864b91-20f4-43e7-b5de-b7e0b724b35f" />


---

## Шаг 5. Редактирование README.md

Был создан и отредактирован файл README.md с основной информацией о проекте.

### Скриншот

<img width="806" height="539" alt="5 1" src="https://github.com/user-attachments/assets/5cfc1e39-6890-41ee-936f-94b813bd12c2" />
_______________________________________________________
<img width="816" height="593" alt="5 2" src="https://github.com/user-attachments/assets/4b87f440-410f-4938-b41c-e87d72c68ea4" />
_______________________________________________________
<img width="626" height="388" alt="5 3" src="https://github.com/user-attachments/assets/af13cf14-bc60-4ac1-bfa4-6ebfa42b8183" />



---

## Шаг 6. Создание ветки feature1

Для разработки мобильного приложения была создана отдельная ветка feature1.

Использованные команды:

```bash id="v99a6m"
git checkout -b feature1
git branch
```

### Скриншот

<img width="1342" height="593" alt="9_github_feature1" src="https://github.com/user-attachments/assets/897d86bc-e405-4129-aafa-6aa2e4afbceb" />



---

## Шаг 7. Создание файла .gitignore

Для исключения служебных файлов Xcode был создан файл .gitignore.

### Скриншот

<img width="1365" height="695" alt="6" src="https://github.com/user-attachments/assets/c992fdf8-d066-44e2-bf82-950bb1c44569" />


---

## Шаг 8. Проверка файлов проекта

Была выполнена проверка структуры файлов проекта.

<img width="526" height="160" alt="7" src="https://github.com/user-attachments/assets/99f53a76-517e-40cf-9fc6-da3a500ebba9" />

---

## Шаг 9. Отправка ветки feature1 на GitHub

Ветка feature1 была загружена в удалённый репозиторий GitHub.

Использованные команды:

```bash id="x90j2h"
git push --set-upstream origin feature1
```

### Скриншот

<img width="529" height="324" alt="12" src="https://github.com/user-attachments/assets/5d834aee-08d7-4a54-b0f3-ed0466a5833b" />


---

# Выполнение задания 1

## Шаг 10. Клонирование репозитория на macOS

На компьютере с macOS был выполнен перенос проекта из GitHub с помощью команды git clone.

Использованные команды:

```bash id="jlwm4n"
git clone https://github.com/...
git checkout -b feature1 origin/feature1
```

### Скриншот

<img width="995" height="197" alt="13" src="https://github.com/user-attachments/assets/ff41d134-c784-4492-ae76-69b8d996b368" />
________________________________________________________
<img width="992" height="222" alt="14" src="https://github.com/user-attachments/assets/6635bda9-60bd-4d04-a2ba-2d1deefd316e" />



---

## Шаг 11. Создание проекта в Xcode

В среде Xcode был создан новый iOS проект на языке Swift.

Параметры проекта:

* Interface — Storyboard
* Language — Swift

### Скриншот

<img width="1280" height="822" alt="16" src="https://github.com/user-attachments/assets/1438e037-58ba-4e95-a896-8388330baf2c" />

<img width="747" height="543" alt="17" src="https://github.com/user-attachments/assets/b9d88f8e-673c-4691-aa61-500f2121ebf4" />



---

## Шаг 12. Создание пользовательского интерфейса

На сцену Main.storyboard были добавлены элементы:

* UILabel
* UISwitch

### Скриншот

<img width="1280" height="828" alt="18" src="https://github.com/user-attachments/assets/54009912-1c5f-4227-ba98-35a45a4826a7" />


---

## Шаг 13. Создание IBOutlet

Для элементов интерфейса были созданы IBOutlet-связи.

Созданные элементы:

```swift id="y1kef5"
@IBOutlet weak var backgroundSwitch: UISwitch!
@IBOutlet weak var switchIndicator: UILabel!
```

### Скриншот

<img width="1280" height="720" alt="19" src="https://github.com/user-attachments/assets/ae7cf55a-447c-4f2f-a836-ec4245963fd1" />


---

## Шаг 14. Создание Action

Для переключателя был создан метод обработки события.

Созданный метод:

```swift id="2m7h0k"
@IBAction func backgroundSwitchTapped(_ sender: Any)
```

### Скриншот

<img width="952" height="424" alt="photo_3_2026-05-11_16-52-15" src="https://github.com/user-attachments/assets/fc4f817c-7900-45d6-87bc-e445c2b43226" />

_________________________________________________________
<img width="1280" height="647" alt="photo_2_2026-05-11_16-52-15" src="https://github.com/user-attachments/assets/18dec813-d727-4460-b307-5ae49b5fa7d7" />

_________________________________________________________
<img width="1280" height="720" alt="photo_1_2026-05-11_16-52-15" src="https://github.com/user-attachments/assets/7249c9d4-7cb5-4f62-bf4a-af34fdc654cc" />



---

# Заключение

В ходе лабораторной работы были изучены:

* основы работы с Git и GitHub;
* создание веток Git;
* работа в Xcode;
* создание мобильных приложений на Swift;
* работа с элементами интерфейса;
* создание IBOutlet;
* разработка пользовательского интерфейса мобильного приложения.

В результате были разработаны:

1. Приложение для смены фона с помощью UISwitch.
2. Приложение для расчёта BMI и BMR.
