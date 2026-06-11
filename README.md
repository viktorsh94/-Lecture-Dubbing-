project-dubbing/
├── README.md
├── requirements.txt
├── Dockerfile
├── inference.ipynb
├── train.py
├── src/
│   ├── __init__.py
│   ├── audio_utils.py
│   ├── ast_pipeline.py
│   ├── tts_pipeline.py
│   └── sync_utils.py
├── results/
│   ├── sample_input.mp4
│   ├── sample_output.mp4
│   └── metrics_report.csv
├── docs/
│   └── report.pdf
└── weights/
    └── (ссылки на модели) 


    
 # Lecture Dubbing Pipeline

## Задача
Автоматизированный дубляж лекций с русского на английский с сохранением синхронизации аудио и видео.

## Особенности решения
* Pipeline № 2: AST → TTS
* Контроль длительности сегментов (±100 мс)
* Нормализация громкости
* Поддержка lip‑sync (опционально)

## Инструкция по запуску

### Вариант 1: Google Colab (рекомендуется)
1. Откройте `inference.ipynb` в Colab.
2. Запустите ячейки последовательно.
3. Загрузите видео в папку `input/`.

### Вариант 2: Локально

**Установка зависимостей:**
```bash
pip install -r requirements.txt

