![Xcode](https://img.shields.io/badge/Xcode-007ACC?style=for-the-badge&logo=Xcode&logoColor=white)
![Swift](https://img.shields.io/badge/swift-F54A2A?style=for-the-badge&logo=swift&logoColor=white)
![IOS](https://img.shields.io/badge/iOS-000000?style=for-the-badge&logo=ios&logoColor=white)
<br/>
![Target](https://img.shields.io/badge/iOS-16.0-blue)
![Version](https://img.shields.io/badge/version-2.0.0-blue)
<br/>
![UIKit](https://img.shields.io/badge/-UIKit-blue)
![SwiftUI](https://img.shields.io/badge/-SwiftUI-blue)
![XIB](https://img.shields.io/badge/-XIB-blue)
![VIPER](https://img.shields.io/badge/-VIPER-blue)
![MVP](https://img.shields.io/badge/-MVP-blue)
![MVVM](https://img.shields.io/badge/-MVVM-blue)
![GCD](https://img.shields.io/badge/-GCD-blue)
![CoreData](https://img.shields.io/badge/-CoreData-blue)
![AutoLayout](https://img.shields.io/badge/-AutoLayout-blue)
![UnitTests](https://img.shields.io/badge/-UnitTests-blue)
<br/>
![SPM](https://img.shields.io/badge/-SPM-blue)
![SwiftLint](https://img.shields.io/badge/-SwiftLint-blue)
![XcodeCloudCI](https://img.shields.io/badge/-XcodeCloudCI-blue)

# Аптечка v2
Второе учебное приложение.

## Screenshots
<img src="https://github.com/ZyFun/MedicineV2/blob/main/Screenshots/Screenshot000.png" width="252" height="497" /> <img src="https://github.com/ZyFun/MedicineV2/blob/main/Screenshots/Screenshot001.png" width="252" height="497" /> <img src="https://github.com/ZyFun/MedicineV2/blob/main/Screenshots/Screenshot002.png" width="252" height="497" /> <img src="https://github.com/ZyFun/MedicineV2/blob/main/Screenshots/Screenshot003.png" width="252" height="497" />

### Splash screen
<img src="https://github.com/ZyFun/MedicineV2/blob/main/Screenshots/Demo.gif" width="252" height="545" />

## Description
Улучшение заключается в том, что теперь лекарства можно распределять по разным аптечкам (домашняя, в автомобиле, в рюкзаке). В первой версии это был единый список. А так же код стал значительно чище и лучше по сравнению с прошлой реализацией.

Затраченное время – сюда не пишу, но смогу сказать точное, установил таймер и отслеживаю затраченное время на каждую задачу, которое записываю в **Jira**.

### Описание используемых технологий
- Многопоточность приложения построена на **GCD**.
- Стараюсь использовать все принципы чистого кода, **DRY, KISS, YAGNI, SOLID и SOA** (Всё еще не идеально. I'm just learning 😅).
- Приложение написано на архитектуре **VIPER**. Пока кривенько, но постепенно переписывается. Это первый проект на этой архитектуре. В этой архитектуре у данного приложения нет необходимости, я использую её только для практики и закрепления навыков. Понимаю, что для данного приложения вполне было бы достаточно MVC или MVP, к примеру с координатором. Но с развитием, простые модули начал писать на **MVP**.
- Для хранения данных используется **CoreData**.
- Для более удобной работы с таблицами с **CoreData** применяется **NSFetchedResultsControll**
- Код частично покрыт Unit тестами.
- Настроен **CI Xcode Cloud** для автоматического запуска тестов.
- Частично, интерфейс написан кодом с помощью **AutoLayout**.
- Вместо **Storyboard** использую **XIB** файлы. 1 экран – 1 **XIB**. В дальнейшем всё будет переделываться под верстку кодом.
- Для подключения фреймворков используется **CocoaPods**
- Часто используемый в разных проектах код, вынесен в **SPM**
- Используется фреймворк **Swiftlint** с кастомными настройками, рекомендованными Тинькофф Образованием + дополнительно своя конфигурация с более жесткими требованиями к стилю кода.
- Весь дизайн приложения был взять из головы.


## News
**22.03.2025**
<br/>
*v.1.5.0*
<br/>
Исправления:
- исправлена ошибка, из-за которой уведомления могли приходить повторно даже при отключенном повторе
- исправлена ошибка, из-за которой при старте приложения отображалось название на другом языке

Остальное:
- различные улучшения и оптимизации в коде
