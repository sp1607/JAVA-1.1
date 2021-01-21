# Отчёт о тестировании KeyValidator 


## KeyValidator - приложение, проверяющее лицензионные ключи.

### Что нужно проверить:

1. Инструкция по установке OpenJDK11 работает под вашу ОС
2. Приложение запускается и совместимо с Java 11
3. Приложение работает согласно руководству использования

21.01.2021 было проведено функциональное тестирование KeyValidator.

На тестирование затрачено: 1 час

В результате тестирования выявлены следующие дефекты:
* [Валидные ключи не прошли валидацию](https://github.com/sp1607/java-1.1/issues/1)
* [Невалидные ключи прошли валидацию](https://github.com/sp1607/java-1.1/issues/2)

## Описание процесса тестирования

**В процессе тестирования использовались следующие артефакты:**
* [Инструкция по установке OpenJDK 11](https://github.com/netology-code/javaqa-homeworks/blob/master/intro/openjdk11-manual.md)
* [Руководство использования](https://github.com/netology-code/javaqa-homeworks/blob/master/intro/user-manual.md)

**В качестве тестовых данных использовались данные из [Руководства использования KeyValidator](https://github.com/netology-code/javaqa-homeworks/blob/master/intro/user-manual.md):**
* 8f05e6a7-70e9-33d7-bfe7-b19eae0d8998 - OK
* 80b427f8-92cd-3aae-ba04-3927fbe17c6  - OK
* b295bc63-9f03-3b4b-af80-969b39f8c262 - OK
* 387eedc6-12e9-3b32-9881-63b6b5e85317 - OK
* c19a8cf9-5c3a-37c5-b7f3-d16d38a0c180 - OK
* 18252235-78e0-44a5-8720-556f0c7da17a - FAIL
* e66075b6-ddad-445e-baf6-161b3289522b - FAIL
* b6d53250-f07e-4352-a293-6102ddf7f1ca - FAIL
* c2bc778a-1cb9-46c6-b435-0489649d2a42 - FAIL
* 2fb98b44-93e7-3bdd-a2ad-79347bfe4ad1 - FAIL

**Тестирование производилось в следующем окружении:**
* ОС: Windows 10 Pro x64
* Java: 11.0.9.1
