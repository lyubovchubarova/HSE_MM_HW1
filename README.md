# Multimodal Image Retrieval for WikiArt

Мультимодальный поиск объектов искусства, включающий в себя 

- поиск похожих изображений с использованием эмбеддингов SIGLip (реализация [здесь](1_img2img.ipynb))
- поиск по текстовым описаниям картин с учетом художника, стиля и жанра (реализация [здесь](2_text2img.ipynb))
- поиск по картинке с текстовым уточнением, включающий в себя zero-shot сгенерированные признаки цветовой гаммы изображения (реализация [здесь](3_omnisearch.ipynb))

Демонстрация работы:

<div align="center">
  <video src="https://github.com/user-attachments/assets/3c9ca6a8-2e7a-4537-98b8-365ce8b74942" />
</div>

Чтобы развернуть приложение локально, нужно открыть `4_gradio_demo.ipynb`, скачать индексы из папки `indices` и запустить все ячейки последовательно

Датасеты хранятся на моем huggingface

- [wikiart_5k](https://huggingface.co/datasets/lyubachuba/wikiart_5k) - основной датасет изображений
- [wikiart_5k_captions](https://huggingface.co/datasets/lyubachuba/wikiart_5k_captions) - сгенерированные подписи
- [wikiart_5k_colors](https://huggingface.co/datasets/lyubachuba/wikiart_5k_colors) - информация о цветовой гамме
