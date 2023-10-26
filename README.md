# frida-tools-termux
<a href="#en">En guide</a>
<a id="ru"></id>
# Ru:
## Шаги установки

1. Обновите пакеты на вашем устройстве:

    ```bash
    pkg update -y && pkg upgrade -y
    ```

2. Установите wget и git:

    ```bash
    pkg install wget git -y
    ```

3. Перейдите на официальный сайт Frida на GitHub: [https://github.com/frida/frida/releases](https://github.com/frida/frida/releases)

4. Скопируйте ссылку на архив с последней версией frida core devtools для вашего устройства. Чтобы узнать архитектуру вашего процессора, выполните команду `uname -m` или `arch`.

5. Введите следующую команду в консоли, чтобы скачать архив:

    ```bash
    wget <ссылка_на_архив>
    ```

6. Создайте папку, где будут храниться файлы Frida:

    ```bash
    mkdir frida-core
    ```

7. Переместите скачанный архив в эту папку:

    ```bash
    mv <имя_архива> frida-core
    ```

8. Перейдите в папку `frida-core`:

    ```bash
    cd frida-core
    ```

9. Распакуйте архив:

    ```bash
    tar -xf <имя_архива>
    ```

10. Определите переменную `FRIDA_CORE_DEVKIT`, указав полный путь до папки `frida-core`. Чтобы узнать текущий путь, выполните команду `pwd`.

    ```bash
    export FRIDA_CORE_DEVKIT=/полный/путь/до/папки
    ```

11. Чтобы сохранить переменную, добавьте ее в файл `.bashrc` и выполните команду `source ~/.bashrc`:

    ```bash
    echo "export FRIDA_CORE_DEVKIT=/полный/путь/до/папки" >> ~/.bashrc
    source ~/.bashrc
    ```

12. Установите frida и frida-tools, используя pip3:

    ```bash
    pip3 install frida frida-tools
    ```

Теперь вы успешно установили Frida в termux. Можете использовать его для разработки и анализа приложений.

<a id="ru"></a>
<a href="en">Ru guide</a>
# En
## Installation Steps

1. Update the packages on your device:

    ```bash
    pkg update -y && pkg upgrade -y
    ```

2. Install wget and git:

    ```bash
    pkg install wget git -y
    ```

3. Go to the official Frida GitHub website: [https://github.com/frida/frida/releases](https://github.com/frida/frida/releases)

4. Copy the link to the archive with the latest version of Frida core devtools for your device. To determine the architecture of your processor, run the command `uname -m` or `arch`.

5. Enter the following command in the console to download the archive:

    ```bash
    wget <archive_link>
    ```

6. Create a folder to store the Frida files:

    ```bash
    mkdir frida-core
    ```

7. Move the downloaded archive to this folder:

    ```bash
    mv <archive_name> frida-core
    ```

8. Navigate to the `frida-core` folder:

    ```bash
    cd frida-core
    ```

9. Unpack the archive:

    ```bash
    tar -xf <archive_name>
    ```

10. Set the `FRIDA_CORE_DEVKIT` variable by specifying the full path to the `frida-core` folder. To find out the current path, run the command `pwd`.

    ```bash
    export FRIDA_CORE_DEVKIT=/full/path/to/folder
    ```

11. To save the variable, add it to the `.bashrc` file and run the command `source ~/.bashrc`:

    ```bash
    echo "export FRIDA_CORE_DEVKIT=/full/path/to/folder" >> ~/.bashrc
    source ~/.bashrc
    ```

12. Install frida and frida-tools using pip3:

    ```bash
    pip3 install frida frida-tools
    ```

You have successfully installed Frida in termux. You can now use it for application development and analysis.
