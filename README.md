# English language version
## Project structure
* `main.py` -- script for MNIST experiment (either Linear or CNN model)
* `rnn_data.py` -- script for RNN experiment
* `trainer.py` -- Trainer class that rules training and encryption stuff
* `distro.py` -- Party and Server classes that knows about model and about encryption and do it
* `distro_paillier/` -- sources of Threshold Paillier Homomorphic Encryption.
I've done minor changes to `decrypt` function for it to work correctly with float numbers.
* `config.py` -- containes singleton config object used by all modules.

## How to run
1. Install system dependencies for crypto stuff: `sudo apt install libgmp-dev libmpfr-dev libmpc-dev`.
2. Install python dependencies: `pip install -r requirements.txt`.
3. Run experiment: `python main.py`.


# Версия на русском языке
## Структура проекта
* `main.py` -- скрипт для эксперимента с MNIST (линейная модель или CNN)
* `rnn_data.py` -- скрипт для эксперимента с RNN
* `trainer.py` -- класс Trainer, который управляет процессом обучения и операциями шифрования
* `distro.py` -- классы Party (Участник) и Server (Сервер), которые содержат логику, связанную с моделью и шифрованием, и выполняют соответствующие операции
* `distro_paillier/` -- исходные коды порогового гомоморфного шифрования Пайе (Threshold Paillier Homomorphic Encryption).
Примечание: Были внесены незначительные изменения в функцию `decrypt`, чтобы она корректно работала с числами с плавающей точкой (float).
* `config.py` -- содержит объект конфигурации в виде синглтона (singleton), используемый всеми модулями.

## Как запустить
1. Установите системные зависимости для криптографических библиотек: `sudo apt install libgmp-dev libmpfr-dev libmpc-dev`.
2. Установите зависимости Python: `pip install -r requirements.txt`.
3. Запустите эксперимент: `python main.py`.
