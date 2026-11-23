<div align="center">

# Folkbench RU

**[ru.folkbench.com][site]** — каталог и замеры API нейросетей для русскоязычных разработчиков

[Сайт][site] · [Каталог][providers] · [Методика][methodology] · [Добавить сервис][submit] · [中文对照](README.zh-CN.md)

</div>

<br>

Открытый репозиторий русскоязычного сайта Folkbench: методика и её ограничения, снимок каталога, каналы для заявок и исправлений, ссылки на тематические подборки. Folkbench не разрабатывает модели и не продаёт доступ к API.

Основной сайт Folkbench — [folkbench.com](https://folkbench.com) (на китайском), его репозиторий — [Folkbench/folkbench](https://github.com/Folkbench/folkbench). У русскоязычного сайта свой каталог, свои замеры и этот репозиторий.

## Что здесь есть и чего нет

**Есть:**

- каталог API-сервисов, проверенных администратором вручную, — с датой проверки;
- автоматические замеры доступности и времени до первого токена (TTFT) с указанием узла и окна статистики;
- методика и её ограничения;
- снимок каталога (ниже) и ссылки на тематические репозитории.

**Нет:**

- данных в реальном времени: таблица ниже — опубликованный снимок, на сайте цифры свежее;
- общего рейтинга «лучший сервис для всех моделей»: сравнивать имеет смысл одну и ту же модель;
- гарантий доступности сервиса или сохранности ваших средств: попадание в каталог — не поручительство за провайдера.

## Как сравнивать

- Сравнивайте одну и ту же модель: точный model ID, протокол, условия оплаты, дату проверки.
- **«Не проверено» не значит «нет».** Отсутствие цены не означает бесплатный доступ.
- «Принимает карты» и «можно оплатить картой российского банка» — разные утверждения. Публикуются только способы оплаты, которые администратор проверил сам.
- Доступность — доля успешных ответов среди всех попыток за 24 часа; ответы 429 и таймауты считаются неуспешными.
- Один замер или один процент доступности не доказывает, что модель подменили, — как и обратного. Отпечаток модели — ранжирование внутри эталонного банка, а не доказательство подлинности её весов.
- Начинайте с минимального пополнения: место в таблице сегодня не гарантирует, что сервис будет работать завтра.

Подробно — в [методике][methodology].

## Когда и откуда сделаны замеры

- Над таблицей всегда указаны номер снимка, время данных (UTC), узел замеров и окно статистики.
- Замеры идут с одного узла. Из вашей сети задержка и доступность могут отличаться.
- Автозамер — короткий запрос: инструменты (tools), кэширование промптов и длинный контекст в него не входят.

## Разделы сайта

| Раздел | Что там |
| --- | --- |
| [Сравнение][site] | Таблицы по моделям: доступность, TTFT, цена, оплата |
| [Каталог провайдеров][providers] | Карточки сервисов: API Base URL, модели, протоколы, проверенные условия |
| [Проверить свой API][workbench] | Тест с пеликаном и сравнение скорости доступны; отпечаток модели на сайте пока не подключён (нет эталонных данных). Ключ не сохраняется |
| [Подключение Claude Code][setup] | Переменные окружения для своего провайдера |
| [Методика][methodology] | Как и откуда мы измеряем, правило сортировки, ограничения |
| [Блог][blog] | Статьи о работе с API нейросетей |
| [Добавить сервис][submit] | Условия и стоимость размещения, шаблон заявки, исправления |

## Сервисы в каталоге

Таблица — копия публичного снимка каталога, а не живые данные базы. Порядок — по названию, это не рейтинг; строки не отбрасываются по имени сервиса.

<!-- ru-catalog:start — генерируется scripts/ru-readme.mjs, не править вручную -->
Снимок `7c49e5ce34a91628` · данные на 23.11.2026, 05:55 UTC · узел US-West · окно 24 часа · порядок — по названию, это не рейтинг.

| Сервис | Модель | Протокол | Доступность 24 ч | TTFT p50 | Цена | Оплата | Проверено |
| --- | --- | --- | ---: | ---: | --- | --- | --- |
| [Modelflare](https://ru.folkbench.com/providers/modelflare/?utm_source=github&utm_medium=referral&utm_campaign=ru_matrix_v1&utm_content=ru_hub_readme) | [`claude-fable-5-2`](https://ru.folkbench.com/models/claude-fable-5-2/?utm_source=github&utm_medium=referral&utm_campaign=ru_matrix_v1&utm_content=ru_hub_readme) | Anthropic Messages | 97,9 % (144 попытки) | 853 мс | не проверена | не проверено | 21.11.2026 |
| [Modelflare](https://ru.folkbench.com/providers/modelflare/?utm_source=github&utm_medium=referral&utm_campaign=ru_matrix_v1&utm_content=ru_hub_readme) | [`claude-opus-5-5`](https://ru.folkbench.com/models/claude-opus-5-5/?utm_source=github&utm_medium=referral&utm_campaign=ru_matrix_v1&utm_content=ru_hub_readme) | Anthropic Messages | 98,6 % (144 попытки) | 848 мс | не проверена | не проверено | 21.11.2026 |
| [Modelflare](https://ru.folkbench.com/providers/modelflare/?utm_source=github&utm_medium=referral&utm_campaign=ru_matrix_v1&utm_content=ru_hub_readme) | [`claude-sonnet-5-5`](https://ru.folkbench.com/models/claude-sonnet-5-5/?utm_source=github&utm_medium=referral&utm_campaign=ru_matrix_v1&utm_content=ru_hub_readme) | Anthropic Messages | 97,9 % (144 попытки) | 926 мс | не проверена | не проверено | 21.11.2026 |
| [Modelflare](https://ru.folkbench.com/providers/modelflare/?utm_source=github&utm_medium=referral&utm_campaign=ru_matrix_v1&utm_content=ru_hub_readme) | [`gemini-4-carbon`](https://ru.folkbench.com/models/gemini-4-carbon/?utm_source=github&utm_medium=referral&utm_campaign=ru_matrix_v1&utm_content=ru_hub_readme) | OpenAI Chat Completions | 100,0 % (144 попытки) | 1 080 мс | не проверена | не проверено | 21.11.2026 |
| [Modelflare](https://ru.folkbench.com/providers/modelflare/?utm_source=github&utm_medium=referral&utm_campaign=ru_matrix_v1&utm_content=ru_hub_readme) | [`gemini-4-hydrogen`](https://ru.folkbench.com/models/gemini-4-hydrogen/?utm_source=github&utm_medium=referral&utm_campaign=ru_matrix_v1&utm_content=ru_hub_readme) | OpenAI Chat Completions | 98,6 % (144 попытки) | 955 мс | не проверена | не проверено | 21.11.2026 |
| [Modelflare](https://ru.folkbench.com/providers/modelflare/?utm_source=github&utm_medium=referral&utm_campaign=ru_matrix_v1&utm_content=ru_hub_readme) | [`gemini-4-neon`](https://ru.folkbench.com/models/gemini-4-neon/?utm_source=github&utm_medium=referral&utm_campaign=ru_matrix_v1&utm_content=ru_hub_readme) | OpenAI Chat Completions | 98,6 % (144 попытки) | 1 129 мс | не проверена | не проверено | 21.11.2026 |
| [Modelflare](https://ru.folkbench.com/providers/modelflare/?utm_source=github&utm_medium=referral&utm_campaign=ru_matrix_v1&utm_content=ru_hub_readme) | [`gpt-6-astra`](https://ru.folkbench.com/models/gpt-6-astra/?utm_source=github&utm_medium=referral&utm_campaign=ru_matrix_v1&utm_content=ru_hub_readme) | OpenAI Chat Completions | 97,9 % (144 попытки) | 1 153 мс | не проверена | не проверено | 21.11.2026 |
| [Modelflare](https://ru.folkbench.com/providers/modelflare/?utm_source=github&utm_medium=referral&utm_campaign=ru_matrix_v1&utm_content=ru_hub_readme) | [`gpt-6.1-sol`](https://ru.folkbench.com/models/gpt-6.1-sol/?utm_source=github&utm_medium=referral&utm_campaign=ru_matrix_v1&utm_content=ru_hub_readme) | OpenAI Chat Completions | 98,6 % (144 попытки) | 849 мс | не проверена | не проверено | 21.11.2026 |
| [Modelflare](https://ru.folkbench.com/providers/modelflare/?utm_source=github&utm_medium=referral&utm_campaign=ru_matrix_v1&utm_content=ru_hub_readme) | [`gpt-6.2-astra`](https://ru.folkbench.com/models/gpt-6.2-astra/?utm_source=github&utm_medium=referral&utm_campaign=ru_matrix_v1&utm_content=ru_hub_readme) | OpenAI Chat Completions | 99,3 % (144 попытки) | 832 мс | не проверена | не проверено | 21.11.2026 |
| [Modelflare](https://ru.folkbench.com/providers/modelflare/?utm_source=github&utm_medium=referral&utm_campaign=ru_matrix_v1&utm_content=ru_hub_readme) | [`gpt-6.2-sol`](https://ru.folkbench.com/models/gpt-6.2-sol/?utm_source=github&utm_medium=referral&utm_campaign=ru_matrix_v1&utm_content=ru_hub_readme) | OpenAI Chat Completions | 98,6 % (144 попытки) | 1 198 мс | не проверена | не проверено | 21.11.2026 |
| [Modelflare](https://ru.folkbench.com/providers/modelflare/?utm_source=github&utm_medium=referral&utm_campaign=ru_matrix_v1&utm_content=ru_hub_readme) | [`grok-4.6`](https://ru.folkbench.com/models/grok-4.6/?utm_source=github&utm_medium=referral&utm_campaign=ru_matrix_v1&utm_content=ru_hub_readme) | OpenAI Chat Completions | 99,3 % (144 попытки) | 1 037 мс | не проверена | не проверено | 21.11.2026 |
| [Modelflare](https://ru.folkbench.com/providers/modelflare/?utm_source=github&utm_medium=referral&utm_campaign=ru_matrix_v1&utm_content=ru_hub_readme) | [`grok-4.7`](https://ru.folkbench.com/models/grok-4.7/?utm_source=github&utm_medium=referral&utm_campaign=ru_matrix_v1&utm_content=ru_hub_readme) | OpenAI Chat Completions | 97,2 % (144 попытки) | 1 231 мс | не проверена | не проверено | 21.11.2026 |
<!-- ru-catalog:end -->

Таблицу собирает скрипт [`scripts/ru-readme.mjs`](scripts/ru-readme.mjs) из [публичного снимка каталога](https://ru.folkbench.com/api/v1/public/catalog). Руками её не правят: данные хранятся в базе сайта, исправления присылайте по каналам ниже. Полные карточки — в [каталоге на сайте][providers].

## Как обновляется этот репозиторий

- Данные каталога хранятся в базе ru.folkbench.com; замеры на сайте идут по его собственному расписанию.
- Таблица здесь обновляется отдельным заданием GitHub Actions, обычно раз в сутки. Если снимок недоступен или не прошёл проверку формата, остаётся последняя удачная таблица, поэтому время над таблицей может отставать от сайта. Ориентируйтесь на это время, а не на дату коммита.
- Все изменения видны в [истории коммитов](../../commits/main).

## Реклама и партнёрские ссылки

- Сайт зарабатывает на платном размещении в каталоге, рекламе и партнёрских ссылках. Рекламные места всегда помечены словом «Реклама» и не входят в таблицы.
- Порядок строк и результаты замеров нельзя изменить за деньги: рекламодатели измеряются тем же запросом и с того же узла, что и остальные.
- Переходы на сайты провайдеров идут через промежуточную страницу `/go/` и могут содержать партнёрский параметр (AFF).
- В этом репозитории рекламы нет.

Подробно — в разделе [«Реклама и партнёрские ссылки»][ads] методики.

## Добавить сервис или исправить ошибку

- **Почта:** reply@folkbench.com
- **Telegram:** [@mmmagnus98](https://t.me/mmmagnus98)
- **GitHub:** [«Folkbench RU: предложить сервис»](../../issues/new?template=ru-add-service.yml) · [«Folkbench RU: исправление»](../../issues/new?template=ru-correction.yml)

Условия, стоимость размещения и порядок проверки — на [странице «Добавить сервис»][submit]. Оплата размещения не влияет на порядок в таблицах. Issues и pull request — только предложения: данные в базу вносит администратор после проверки источника. Результаты замеров по запросу не меняются: если замер ошибочен, мы исправляем причину, а не цифру.

**Не публикуйте API-ключи, пароли, платёжные данные и личные документы.** Issues открыты всем.

## Тематические репозитории

Ведутся отдельно, это редакционные подборки, а не данные каталога:

- [awesome-ai-guide-ru](https://github.com/Folkbench/awesome-ai-guide-ru) — руководства: официальные ограничения доступа, подписки, оплата, проверка API до покупки.
- [relay-api-ru](https://github.com/Folkbench/relay-api-ru) — каталог API по публичным источникам и [редакционное сравнение](https://folkbench.github.io/relay-api-ru/).
- [awesome-free-ai-ru](https://github.com/Folkbench/awesome-free-ai-ru) — бесплатные ресурсы: условия freemium-API, локальные движки и открытые веса. Облачные лимиты, локальные инструменты и сами модели там разделены.

## Лицензия

Оригинальные тексты и изображения Folkbench в этом репозитории — [CC BY 4.0](LICENSE-CC-BY-4.0.txt); наши скрипты — [MIT](LICENSE-MIT.txt). Подробное разграничение, в том числе почему снимок каталога в таблице не объявляется целиком лицензированным по CC, — в [LICENSE.md](LICENSE.md). Названия и товарные знаки сервисов и моделей принадлежат их владельцам и этими лицензиями не передаются.

[site]: https://ru.folkbench.com/?utm_source=github&utm_medium=referral&utm_campaign=ru_matrix_v1&utm_content=ru_hub_readme
[providers]: https://ru.folkbench.com/providers/?utm_source=github&utm_medium=referral&utm_campaign=ru_matrix_v1&utm_content=ru_hub_readme
[workbench]: https://ru.folkbench.com/?utm_source=github&utm_medium=referral&utm_campaign=ru_matrix_v1&utm_content=ru_hub_readme#workbench
[setup]: https://ru.folkbench.com/setup/claude-code/?utm_source=github&utm_medium=referral&utm_campaign=ru_matrix_v1&utm_content=ru_hub_readme
[methodology]: https://ru.folkbench.com/methodology/?utm_source=github&utm_medium=referral&utm_campaign=ru_matrix_v1&utm_content=ru_hub_readme
[ads]: https://ru.folkbench.com/methodology/?utm_source=github&utm_medium=referral&utm_campaign=ru_matrix_v1&utm_content=ru_hub_readme#ads
[blog]: https://ru.folkbench.com/blog/?utm_source=github&utm_medium=referral&utm_campaign=ru_matrix_v1&utm_content=ru_hub_readme
[submit]: https://ru.folkbench.com/submit/?utm_source=github&utm_medium=referral&utm_campaign=ru_matrix_v1&utm_content=ru_hub_readme
