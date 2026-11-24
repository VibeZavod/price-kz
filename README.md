# price-kz — скилл Claude: где купить дешевле в Алматы

Скилл для Claude, который ищет цену товара для покупателя в Алматы: Kaspi и другие площадки
Казахстана, Россия, Китай (Pinduoduo, Taobao, AliExpress), США и Европа. Итог — в тенге «до двери»:
с доставкой, пошлиной, курсом Нацбанка РК, гарантией и отзывами на модель. Ничего не покупает.

## Установка одной фразой (Claude Code)

Вставь в Claude Code:

```
Установи скилл price-kz: склонируй https://github.com/VibeZavod/price-kz в ~/.claude/skills/price-kz
(если папка уже есть — сделай там git pull). Проверь, что внутри лежит SKILL.md, и скажи,
что после перезапуска Claude Code скилл заработает по фразам «сколько стоит», «где купить дешевле».
```

Или руками:

```sh
git clone https://github.com/VibeZavod/price-kz ~/.claude/skills/price-kz
```

Обновить: `git -C ~/.claude/skills/price-kz pull`.

## Claude в браузере или в приложении (чат)

1. Скачай `price-kz.zip` со страницы [Releases](https://github.com/VibeZavod/price-kz/releases/latest).
2. Settings → Capabilities → включи выполнение кода.
3. Customize → Skills → «+» → Upload a skill → выбери `price-kz.zip`.

## Что нужно для полной работы

- **Claude in Chrome** (расширение) — Kaspi, Ozon, Pinduoduo и Amazon не отдают страницы роботам,
  скилл читает их через твой браузер. Без него цены будут помечены «не проверено».
- Pinduoduo и Taobao — один раз войти в свой аккаунт в Chrome; скилл подскажет как.

Растаможка в скилле проверена 24.11.2026; через 60 дней скилл сам попросит её перепроверить.
