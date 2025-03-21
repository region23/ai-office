# AI Office: Open Source YouTube-Show

![Заставка](media/cover_1.jpeg "AI Office Team")

> **AI Office** — это экспериментальное шоу, в котором команда ИИ-агентов (CEO, CTO, разработчики, маркетологи и др.) создают реальный продукт от идеи до релиза, а зрители влияют на сюжет. Цель проекта — объединить искусственный интеллект, ситком-повествование, коллективную разработку и показать, как «виртуальный стартап» может реально генерировать код и бизнес-идеи. Сюжет подан в комедийно-сатирическом ключе, вдохновлен стилеобразующими элементами сериала «Кремниевая долина» – с высмеиванием стереотипов IT-индустрии, неуклюжими ситуациями в команде и мета-иронией над хайпом вокруг технологий. В каждом эпизоде присутствует разнообразие юмористических ситуаций на фоне общей сквозной истории разработки продукта. Сериал стилизован под эстетику мультсериала The Midnight Gospel (психоделический, яркий стиль), с балансом роботических и человеческих черт (TBD).

## Коротко об идее

- **ИИ-агенты**: Каждый персонаж — это отдельный агент со своей ролью (CEO, CTO, Dev, маркетолог и т. д.), у которого прописаны навыки, характер и приоритеты.
- **Процесс разработки**: Агенты получают задачу (например, придумать идею стартапа), ищут информацию через интернет, спорят и формируют решения.
- **Открытый код**: Всё, что агенты «написали» (Python, Vue и пр.), будет доступно в репозитории. Сообщество может использовать/улучшать этот код.
- **Сериал**: Из логов общения агентов формируется сюжет, раскадровка с описанием каждой сцены, включая локации, персонажей и ключевые действия. (обработанный специальными сценарными агентами + людьми-редакторами), а затем генерируется анимация и озвучка.
- **Интерактивность**: Зрители голосуют за решения, подсказывают идеи и напрямую влияют на будущие эпизоды.

## Зачем это нужно?

1. **Развлечение и обучение**: Показать процесс стартап-разработки сквозь призму юмора.  
2. **Эксперимент с ИИ**: Продемонстрировать, как несколько агентов могут совместно работать над реальными задачами, писать код, генерировать сценарии.  
3. **Open Source**: Создать открытую платформу, к которой любой желающий может присоединиться, внести свой вклад, обучиться передовым инструментам ИИ и разработки.  

## Основные элементы

- **OpenAI Agents SDK** (или аналог): логика «ролевых» ИИ, умеющих обращаться к внешним инструментам (Tools).  
- **Flask + Vue 3**: веб-платформа для интерактивного участия зрителей: голосования, просмотр логов, комментарии.  
- **Анимация и озвучка**: ComfyUI, Sora/Kling для простых анимированных роликов, TTS и lip-sync (Wav2Lip) для синхронизации голосов.

## Как это работает в общих чертах

1. **Итерация (эпизод)**:  
   - CEO даёт задание (например, «придумайте идею, чтобы заработать на подписке»).  
   - Агенты обмениваются сообщениями, спорят, пользуются интернетом (Tools), анализируют рынок, выбирают продукт.  
   - Сгенерированный код (MVP) складывается в репозиторий.  
   - Формируется лог диалогов.
2. **Сценарная обработка**:  
   - Из лога создаётся «черновой» сценарий специальным агентом-сценаристом и раскадровка с описанием каждой сцены, включая локации, персонажей и ключевые действия (возможно другим агентом, специально под это заточенным).  
   - Человек-редактор (Script Advisor) доводит материал до комедийного вида.  
   - Аватары генерируются (Midjourney + Sora/Kling), озвучка — TTS, синхронизация губ — Wav2Lip.
3. **Выпуск серии**:  
   - 5–10-минутный ролик на YouTube.  
   - Зрители голосуют и комментируют на платформе, влияя на сюжет следующего эпизода.  

## Текущий статус

- **Состояние**: Проект на стадии разработки. Пилотная конфигурация агентов и базовая платформа в процессе сборки.  
- **Что готово**:
  - Черновая структура для ИИ-агентов.  
  - Базовые шаблоны Flask + Vue.  
  - Простейший конвейер генерации сценария.  
- **Что нужно доработать**:
  - Расширенная логика ролей и характеров агентов.  
  - Модуль самоорганизации и фракций.  
  - Полный pipeline анимации + озвучки.  

## Артефакты
- [Техническое Задание на разработку платформы проекта AI Office](specification.md)
- [Персонажи "AI Office" и локации](characters_and_locations.md)
- [Рекомендации по созданию персонажей и анимации](images_and_animation.md)

## Как поучаствовать

1. Форкните репозиторий и начните эксперименты с логикой агентов или улучшите веб-платформу.  
2. Открывайте Issue с предложениями, багами или идеями новых фич.  
3. Предлагайте Pull Request с доработками (очень приветствуется!).  
4. Присоединяйтесь к обсуждениям, участвуйте в голосованиях.

## Лицензия

Проект распространяется под лицензией [Creative Commons Attribution-NonCommercial-ShareAlike 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/deed.ru). Вы можете свободно использовать код, модифицировать его и вносить свой вклад. Просим сохранять упоминание авторов и соблюдать условия лицензии.



## Обратная связь и планы

- Всех заинтересованных приглашаем создавать Issues, предлагать Pull Requests и тестировать функциональность.  
- Любые идеи по развитию логики агентов, сценарию, анимации — приветствуются!  
- Планы на будущее:
  - Улучшить генерацию сценариев и добавить больше «человеческих» крючков для юмора.  
  - Реализовать более гибкую систему репутации агентов.  
  - Подключить новые способы монетизации (аккуратно, без агрессивной рекламы).

---

## Заключение

**AI Office** — это амбициозный проект на стыке ИИ, сериалов и опенсорс-сообщества. Мы приглашаем всех, кто хочет поэкспериментировать с мультимодальными генеративными моделями, поучаствовать в создании уникального «виртуального стартапа» и увидеть, как искусственный интеллект может **не только** генерировать тексты, **но и** разрабатывать работоспособные продукты (пусть и с помощью «человеческого» надзора).

Добро пожаловать!  

— *Команда AI Office*  