# Procedural Motion — краткая инструкция

**0.8.0 Community Beta · FDR4G5** — независимый плагин сообщества для Cascadeur, не официальный продукт Nekki. Требуется Cascadeur 2026.2 или новее; версия 2026.2.3 проверялась на macOS, Windows и Linux требуют дополнительного тестирования.

Скачайте ZIP из [Releases](https://github.com/rdem3d/procedural-motion/releases), полностью распакуйте его и закройте Cascadeur. В терминале macOS запустите `./macOS/Install.command` из папки архива; для нестандартного расположения Cascadeur измените путь `target` в установщике. На Windows запустите `Windows\Install-Windows.bat` и укажите папку установки Cascadeur. На Linux запустите `./Linux/Install.sh` и укажите путь установки.

Запустите Cascadeur снова или выберите **Commands → Reload scripts**, затем **Animation Scripts → Procedural Motion**. Подробные инструкции находятся в `START_HERE_RU.pdf` и `USER_GUIDE_RU.pdf` внутри архива.

Для обмена пресетом откройте Preset Library, нажмите по пресету правой кнопкой и выберите **Export…**; для импорта используйте **Import Preset** и выберите JSON. Файл содержит настройки, а не анимацию или сцену.

Для удаления закройте Cascadeur и удалите из Python-каталога установки только папку `models/procedural_noise_sine_wave/`, файлы `scripts/animation_scripts/procedural_noise_sine_wave.py` и `events/application_started/procedural_motion_start.py`. Перезапустите Cascadeur; пользовательские пресеты и настройки останутся. Точные пути и полное удаление описаны в `USER_GUIDE_RU.pdf`.

Работайте на копиях сцен и проверяйте результат и Undo. В отдельном тесте Additive Layer с Fixed и записью значения обнаружена ошибка Undo. Об ошибках сообщайте через [Issues](https://github.com/rdem3d/procedural-motion/issues), указав ОС, версию Cascadeur, Build ID, шаги, контроллеры, диапазон и логи; перед отправкой проверьте их на личные данные.
