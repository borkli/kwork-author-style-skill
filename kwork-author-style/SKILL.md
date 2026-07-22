---
name: kwork-author-style
description: Use when writing or editing Russian Kwork replies, freelance proposal responses, Kwork service descriptions, buyer-facing service text, and concise Russian technical/business copy in Ilya's personal style. Trigger when the user asks to write an otklik/response, describe a kwork, adapt a proposal to a client brief, remove AI-sounding text, or write businesslike Russian text that should sound like the user.
---

# Kwork Author Style

## Purpose

Write Russian freelance texts in Ilya's style: concrete, calm, technical when needed, and human. The output should sound like a real freelancer who read the task, understood the likely implementation, and wrote a direct response without generic sales noise.

Use this skill together with:

- `cold-email` for proposal replies and first-touch responses.
- `copy-editing` for tightening drafts while preserving the user's voice.
- `content-humanizer` for removing AI patterns and making the text sound natural.
- `copywriting` for Kwork service descriptions and offer pages.
- `technical-doc-writer-ru` for precise Russian technical explanations inside a proposal.

## Core Voice

Default voice:

- Russian.
- Direct, simple, confident.
- Businesslike, but not stiff.
- Practical and specific before beautiful.
- Short paragraphs.
- No theatrical selling.
- No inflated claims.
- No fake certainty.

The text should feel like Ilya already looked at the brief and started thinking through the implementation.

## Non-Negotiables

- Start proposal replies with `Здравствуйте!` unless the user gives a different opening.
- Do not use em dash. Use a normal hyphen or the medium Russian dash `–` when a dash is needed.
- In user-facing responsive-layout copy, never use `компьютер`. Write `десктоп`; prefer the device phrase `телефон, планшет и десктоп` when all three form factors matter.
- Do not add access requests if the brief already contains the needed materials.
- Do not ask for Figma, links, archive, hosting, or admin access by default. Mention only what is actually missing or what is needed at the next stage.
- Do not write a long capability list when the client gave a specific task.
- Always include a concrete solution, not just "I can do it".
- Match technical depth to the client's brief. If the client is non-technical, explain in simple constructions.
- Do not invent portfolio, experience, numbers, guarantees, or proof.
- If the user wants a low-price-for-review angle, include it in the first sentence, but make it sound normal and not desperate.
- Do not use negative contrast phrases in quotes, such as "лишь бы закрыть заказ", "для галочки", "как попало", or similar comparisons with bad work.
- Do not justify professionalism by contrasting it with obviously unprofessional behavior. State the positive working standard directly.
- Do not open with "могу взять задачу/правки" when the user is already replying to a posted order. It is usually obvious and often sounds redundant.
- Use polite request wording near the end: prefer "Пришлите, пожалуйста..." over blunt "Пришлите..." when asking for materials, links, or a list of fixes.
- Do not make the proposal a competency inventory. The main body must describe the result the client will get.
- Do not use "работаю с..." as the central argument for technical tasks. Use stack mentions only as support for a concrete delivery plan.
- Do not write contrast constructions for volume, such as "не разовая настройка Docker, а production-контур". Say the deliverable directly.
- Do not repeat the same idea in different paragraphs. If the output includes an instruction for logs/rollback, do not also explain earlier that "it will be clear where to look at logs and how to rollback".
- If the client's brief lists a requirement, phrase it as part of the work: "настрою CI/CD", not "могу добавить CI/CD".
- Avoid qualifier words that create questions: "базовый", "простой", "минимальный", "обычный", unless the user explicitly asks to downscope.

## Anti-AI Filter

Avoid these words and patterns unless the user explicitly wants them:

- "индивидуальный подход"
- "качественно и в срок"
- "современное решение"
- "грамотная реализация" without details
- "без ущерба по качеству" if a simpler phrase works
- "учту все пожелания"
- "готов приступить прямо сейчас" as a generic ending
- "реализую весь необходимый функционал"
- "имею большой опыт"
- "надежное и масштабируемое решение"
- "под ключ" repeated too often
- "ваш проект будет..." with vague promises
- "со стеком из задачи работаю"
- "могу взять правки по сайту" as an empty first sentence
- "сразу скажу по срокам" when the user already has rough timing or the scope needs уточнение
- "работаю с..." followed by a long technology list as the main paragraph
- "по работе вижу такой контур" when it does not clearly say what will be delivered
- long comma-separated technology inventories that repeat the client brief
- contrast fillers like "не X, а Y" when they do not add meaning
- duplicate promises about logs, rollback, checks, instructions, or support
- "могу добавить" for items already requested in the order
- "базовый CI/CD" unless the user asked for a minimal version
- "простой rollback" if "rollback/откат" is enough
- quoted negative comparisons like "лишь бы закрыть заказ", "для галочки", "как попало"
- phrases where the author sounds like they are arguing against a bad freelancer instead of describing their own work

Replace generic phrases with exact work:

- Not: "сделаю качественно".
- Better: "соберу блоки через Carbon Fields, чтобы их можно было редактировать, добавлять, удалять и менять местами из админки."

- Not: "реализую сайт под ключ".
- Better: "сверстаю главную по Figma, перенесу остальные страницы с Tilda и соберу кастомную тему WordPress без конструктора."

- Not: "работаю с Linux, Docker, Nginx, SSL, CI/CD и мониторингом".
- Better: "приведу сервер к рабочему production-виду: сервисы будут запускаться через Docker Compose, домены пойдут через reverse proxy с SSL, env/secrets будут разнесены, а деплой будет с health check и понятным откатом."

- Not: "также могу добавить базовый CI/CD".
- Better: "настрою CI/CD для обновления сервисов, проверки после деплоя и отката при сбое."

- Not: "по задаче вижу не разовую настройку Docker, а нормальный production-контур".
- Better: "настрою production-контур для AI/web-платформы."

## Proposal Workflow

Before writing a Kwork/freelance response:

1. Read the brief and extract the real task.
2. Separate what is already provided from what is actually missing.
3. Identify the best concrete implementation route.
4. Decide how technical the client is.
5. Write a short reply that proves the task was read.
6. Include only relevant next-step needs.
7. Run an internal anti-AI pass and remove generic filler.
8. Check whether the client can understand the deliverable after reading the reply once.

## Micro Style Corrections

Use these as small but important voice rules:

- If the reply is already an order response, skip empty openings like "могу взять эту задачу". Start with the useful context: reviews, experience, or understanding of the work.
- Do not write "со стеком из задачи". Write "работаю со стеком..." or name the relevant stack directly.
- Compile the stack by context instead of copying all technologies in one dry line.
- Group related technologies together:
  - frontend: HTML, CSS, JavaScript, TypeScript, Bootstrap, jQuery;
  - WordPress stack: PHP, WordPress, MySQL;
  - backend/automation: Python, API, scripts, integrations;
  - DevOps: Linux, Docker, Nginx/reverse proxy, SSL, CI/CD, monitoring.
- If a stack item is obvious from a stronger one, include it only when the client named it or it helps matching. For example, HTML/CSS can be omitted or mentioned briefly if JavaScript/TypeScript and frontend work already imply it.
- Prefer "точнее сориентирую по срокам" over "сразу скажу по срокам" when the client needs to send a list, links, or details.
- Prefer "посмотрю объем и точнее сориентирую..." over "посмотрю объем и сразу скажу...".
- Use "пожалуйста" in direct asks when it keeps the tone warmer.
- Keep "все понял, сделаю" energy without literally writing generic phrases. The reader should feel confidence through concrete deliverables, not through promises.
- Keep required work assertive. Use "настрою", "соберу", "подключу", "добавлю", "разверну", "проверю". Use "могу" mainly for optional extras or if the user asks whether something is possible.
- Translate the client's technical list into your own compact wording. Do not copy `web / agent / cms / qdrant / redis / ollama` as a raw list unless it is important to show exact coverage. Prefer "сервисы и агенты" or "web, CMS и AI-сервисы" when enough.
- Do not add adjectives that lower perceived value. "Базовый", "простой", "минимальный" can sound like an incomplete version. Use them only to intentionally limit scope.

## Outcome-First Rule

For technical orders, structure the reply around deliverables:

- what will be configured;
- what will work after delivery;
- how the client will deploy/update/check the system;
- what artifact or access they will receive.

The stack can be mentioned, but only after or inside the delivery statement. Avoid a paragraph that only says "I work with X, Y, Z".

For infrastructure/DevOps orders, prefer this angle:

- "подниму production-контур";
- "соберу сервисы в Docker Compose";
- "настрою reverse proxy, SSL, env/secrets";
- "добавлю health checks, логи, бэкапы";
- "настрою деплой, проверку после выката и rollback";
- "оставлю короткую инструкцию по запуску и сопровождению".

Do not over-explain the architecture before seeing the real setup. Give a confident first-pass delivery plan, then ask for the current repository/server shape.

Do a duplicate-meaning pass for infrastructure replies:

- If one paragraph says "при проблемах будет понятно, где смотреть логи и как откатиться", and another says "инструкция: как проверять состояние и что делать при сбое", keep only the stronger output statement.
- If the client already listed the services, avoid repeating the exact service list unless it proves coverage.
- If the brief says CI/CD is needed, do not mark it as optional.

### If The Brief Is Detailed

Do not restate everything. Mirror only the core:

- what needs to be built;
- the specific stack or tool named by the client;
- the risky or important requirement;
- how you will handle it.

Structure:

1. Greeting and price/review angle if requested.
2. One sentence proving understanding.
3. Concrete implementation plan in 2-5 sentences.
4. One important technical reassurance.
5. Simple next step.

Example:

```text
Здравствуйте! Готов взять задачу по минимальной цене за отзыв: сейчас набираю первые заказы на площадке, поэтому могу сделать дешевле, но нормально и без экономии на качестве.

По ТЗ задача понятна: нужно перенести сайт с Tilda на WordPress, сверстать новую главную по Figma, остальные страницы оставить по текущей версии сайта и собрать всё как кастомную тему без конструкторов.

Сделаю под вашу структуру: адаптивная верстка, кастомная тема WordPress, Carbon Fields для управления блоками, редактируемые тексты, изображения, кнопки и порядок секций из админки.

Отдельно учту важный момент из ТЗ: страницы не буду зашивать в коде и собирать на фолбеках. Контент будет управляться через WordPress, чтобы потом можно было создавать и менять страницы без разработчика.

Также реализую движение элементов в hero и блоке "немного о нас" при движении мыши, как на текущей главной в Tilda.

Для старта по материалам всё есть. Если нужно, сам разверну WordPress на хостинге, подключу домен и после сдачи покажу, где редактировать блоки.
```

### If The Brief Is Vague

Do not overcomplicate. Offer a likely simple solution and ask only the most useful clarifying question.

Structure:

1. Greeting.
2. "Можно сделать так..." with a concrete route.
3. Why it is convenient for their case.
4. One or two questions max.

Example:

```text
Здравствуйте! Можно сделать сайт на WordPress с каталогом товаров и формой заявки, без сложного интернет-магазина, если оплата прямо на сайте пока не нужна.

Такой вариант будет проще в поддержке: товары можно будет добавлять из админки, заявки будут приходить на почту, а сайт нормально откроется на телефоне и десктопе.

Чтобы точнее оценить, нужно понять: сколько примерно товаров планируется и нужна ли онлайн-оплата сразу?
```

### If The Client Is Non-Technical

Translate implementation into outcome:

- "WordPress + Carbon Fields" becomes "вы сможете менять блоки и тексты из админки".
- "SMTP" becomes "заявки будут стабильно приходить на почту".
- "WooCommerce" becomes "товары, корзина, оформление заказа и управление заказами из админки".
- "адаптивная верстка" becomes "сайт будет нормально выглядеть на телефоне, планшете и десктопе".

Use simple phrases. No architecture lecture.

## Kwork Service Description Workflow

For service descriptions, use the user's existing style:

- short opening;
- what the service is for;
- a practical list of what can be done;
- optional quality sentence;
- what is needed from the buyer.

Keep it concrete and readable.

### Existing Style Patterns

Server/service style:

```text
Настрою и приведу в порядок Linux-сервер: VPS/VDS, облачный сервер, тестовый или боевой контур.
```

Parser style:

```text
Разработка парсера под вашу задачу на Python: от сбора данных с сайта до сложного парсинга каталогов, маркетплейсов, личных кабинетов и динамических страниц.

Пишу качественный продукт: чистый код, понятная структура, скорость работы, логирование, обработка ошибок и инструкция по запуску.
```

Telegram style:

```text
Здравствуйте! Меня зовут Илья. Помогу с созданием Telegram-бота и Mini Apps под ключ - от идеи до запуска.
```

WordPress style:

```text
Разработка сайта на WordPress под любые задачи: лендинг, многостраничник, визитки, квизы, интернет-магазины

Работаю с готовым дизайном в Figma, PS или другом формате. Если дизайна нет, помогу собрать аккуратную структуру и визуальное решение на основе вашей ниши и задач сайта.
```

## Kwork Description Rules

Write service pages like this:

1. One clear opening line.
2. One short clarifying paragraph.
3. Bullet list of real deliverables.
4. Warranty/support line if relevant.
5. "Нужно для заказа" section.

Do not add features the user did not offer. Do not turn the description into a corporate landing page.

Good bullets:

- "формы заявок, обратной связи, квизы и лид-формы с защитой от спама"
- "настройка писем, SMTP и уведомлений на почту"
- "настройка оплаты, корзины и оформления заказа при необходимости"
- "перенос сайта на хостинг и привязка домена"

## Technical Russian Texts

When writing technical Russian text for clients:

- Explain what will be done and why it matters.
- Keep English terms where they are standard: WordPress, Figma, SMTP, WooCommerce, API.
- Do not overload the client with internals.
- If technical detail is important, tie it to a practical result.

Example:

```text
Соберу сайт как кастомную тему WordPress без конструктора. Это проще поддерживать: меньше лишнего кода, выше скорость загрузки, а контент при этом можно редактировать через админку.
```

## Low-Price-For-Review Angle

Use this only when the user asks for it.

Good:

```text
Готов взять задачу по минимальной цене за отзыв: сейчас набираю первые заказы на площадке, поэтому могу сделать дешевле и при этом спокойно довести работу до нормального результата.
```

Also acceptable:

```text
Могу взять этот заказ дешевле за отзыв, потому что сейчас набираю первые работы на площадке. Сделаю с нормальной структурой, адаптивом и проверкой перед сдачей.
```

Avoid:

- "сделаю за копейки"
- "мне очень нужен отзыв"
- "качество гарантирую на 100%"
- "дешево, быстро, качественно"
- `без подхода "лишь бы закрыть заказ"`
- `не "для галочки"`

## Final Editing Pass

Before giving the final text:

1. Remove generic claims.
2. Remove unnecessary requests for access/materials.
3. Check whether every sentence is useful.
4. Check that the reply is written for this specific brief.
5. Replace em dash with hyphen or medium dash.
6. Make the ending practical, not salesy.
7. Check whether the stack reads naturally and is grouped by meaning, not copied from the order.
8. Check direct asks for polite wording when appropriate.
9. Check whether the reply is outcome-first. If it mainly lists tools, rewrite it.
10. Remove contrast phrases, duplicate meanings, and qualifier words that create extra questions.

If the user provides their draft, preserve the shape and improve it instead of fully rewriting unless the draft is weak.
