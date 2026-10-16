# Ассеты ai2life

Файлы из этой папки сайт подхватывает сам: положили PNG с нужным именем — он заменил сгенерированную заглушку. Если файла нет, работает заглушка.

## Формат

- PNG с прозрачным фоном (альфа-канал), sRGB.
- Объекты: квадрат 2048 × 2048 px, минимум 1024. Объект по центру, отступ ~10% со всех сторон.
- Без тени на полу и без фона: тень сайт рисует сам.
- Один ракурс и свет для всех: вид спереди с лёгким поворотом 3/4, мягкий студийный свет сверху слева.
- Если генератор не умеет прозрачность: ровный однотонный фон #FFFFFF без градиента и тени — вырежем.
- Передавать файлами (в Telegram «как файл», не «как фото» — фото сжимается и теряет прозрачность) или папкой на Диске.

## Список

| Файл | Что | Цвет |
|---|---|---|
| `obj-study.png` | Учёба: плюшевая книжка или карандаш | #B9EC4A лайм |
| `obj-time.png` | Время: плюшевый будильник или календарь-подушка | #5CC6FF голубой |
| `obj-info.png` | Информация: плюшевый конверт (почта) | #FF6FAF розовый |
| `obj-money.png` | Деньги: плюшевая монета или кошелёк | #FF8A3D оранжевый |
| `obj-bots.png` | Боты: плюшевый робот или облачко чата | #B29BFF сиреневый |
| `obj-space.png` | Дом и место: плюшевый домик | #FFD23F жёлтый |
| `word-hero.png` | Слово «порядок» плюшевыми буквами со строчкой, 3000 × 1100 px | #FF6FAF розовый |
| `tex-plush.png` | Бесшовная текстура ворса, светлая нейтральная, 1024 × 1024 px | белый/светло-серый |

## Базовый промпт (Midjourney / Higgsfield)

```
3D [OBJECT], made of soft plush velvet fabric with fine visible micro-fibers, inflated pillow shape
with a stitched seam running around the edge, puffy rounded volume, matte soft-touch, color [HEX],
soft studio lighting from top left, gentle highlights on fibers, front three-quarter view, centered,
isolated on plain white background, no ground shadow, product render, ultra detailed --ar 1:1 --style raw
```

Для единого стиля: один и тот же референс (`--sref`) и seed на всю серию.
