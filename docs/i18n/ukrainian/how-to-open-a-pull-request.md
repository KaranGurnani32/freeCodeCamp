# Як відкрити запит на злиття (PR)

Запит на злиття (PR) дозволяє надсилати зміни зі свого форку на GitHub до головного репозиторію freeCodeCamp.org. Як тільки ви закінчите вносити зміни до коду, дотримуйтесь цих рекомендацій, щоб відкрити PR.

Ми очікуємо, що наші помічники обізнані щодо процесу проєкту. Ви отримаєте повагу тих, хто відповідає за технічне обслуговування, і заощадите час, дотримуючись цих вказівок.

Деякі приклади:

1. Не редагуйте файли напряму через GitHub, це не дуже хороша ідея.
2. Переконайтесь, що дотримуєтесь контрольного списку PR, а не просто ставите галочки. В такому випадку ми не сприйматимемо вас серйозно.
3. Використовуйте правильний спосіб пов’язати завдання в описі PR, оновивши `XXXXXX`. Не додавайте номери завдань будь-де.
4. Не «@згадуйте» чи запитуйте відгук кілька разів.

   Ми розуміємо, що ви раді зробити свій внесок. Модераторам подобається відповідати кожному, однак пам’ятайте: вони зайняті люди, які розглядають сотні запитів. Рано чи пізно, хтось дійде і до вашого запиту.

5. Не працюйте напряму зі своєї гілки `main`. Створіть нову гілку для змін, над якими ви працюєте.

> [!NOTE] Ваш PR повинен націлюватись лише на зміни навчальної програми англійською мовою. Див. [цей довідник](index.md#translations), щоб зробити внесок до перекладу.

## Prepare a Good PR Title

Ми рекомендуємо використовувати [ загальноприйняті заголовки та повідомлення](https://www.conventionalcommits.org/) для комітів і запитів на злиття. Конвенція вимагає наступного формату:

> `<тип>([область (необов’язково)]): <опис>`
> 
> Наприклад:
> 
> `fix(learn): тести для завдання з циклу do...while`

Щоразу, коли ви відкриваєте запит на злиття (PR), використовуйте нижчеподану інформацію, щоб визначити тип, область та опис.

**Тип:**

| Тип   | Коли обирати                                                               |
|:----- |:-------------------------------------------------------------------------- |
| fix   | Змінені або оновлені/вдосконалені функції, тести, формулювання уроку тощо. |
| feat  | Лише при додаванні нової функції, тестів тощо.                             |
| chore | Зміни, які не повʼязані з кодом, тестами або формулюванням уроку.          |
| docs  | Зміни до каталогу `/docs` чи настанов щодо внесків тощо.                   |

**Область:**

Область можна обрати із [цього списку міток](https://github.com/freeCodeCamp/freeCodeCamp/labels?q=scope).

**Опис:**

Опис повинен бути коротким (не більше 30 символів) та простим; більше інформації можна додати в полі опису PR та коментарях.

Декілька прикладів хороших заголовків:

- `fix(a11y): improved search bar contrast`
- `feat: add more tests to HTML and CSS challenges`
- `fix(api,client): prevent CORS errors on form submission`
- `docs(i18n): fix links to be relative instead of absolute`

## Запропонуйте PR

1. Як тільки зміни будуть збережені, вам буде запропоновано створити PR на сторінці вашої гілки GitHub.

   <details>
   <summary>Переглянути знімок екрану</summary>

   ![Зображення - Порівняння та підказки PR на GitHub](https://contribute.freecodecamp.org/images/github/compare-pull-request-prompt.png)

   </details>

2. Усі PR потрібно надсилати до головного репозиторію freeCodeCamp — гілки `main`.

   Переконайтеся, що значення base fork встановлено на freeCodeCamp/freeCodeCamp під час створення PR.

   <details>
   <summary>Переглянути знімок екрану</summary>

   ![Зображення - Порівняння форків під час створення PR](https://contribute.freecodecamp.org/images/github/comparing-forks-for-pull-request.png)

   </details>

3. Надішліть PR зі своєї гілки до гілки freeCodeCamp `main`.

4. У тілі свого PR вкажіть детальну інформацію про внесені зміни та чим вони корисні.

   - Вам буде надано шаблон PR. Це список, якого потрібно дотримуватись перед відкриттям PR.

   - Заповніть деталі, які ви вважаєте за потрібне. Ця інформація буде розглянута, а модератори вирішать, чи ваш PR буде прийнятий.

   - Якщо PR призначений для вирішення наявного завдання на GitHub, то використайте ключове слово _Closes_ та номер завдання в кінці опису, щоб [автоматично закрити цю проблему, якщо PR прийнятий та об’єднаний](https://help.github.com/en/articles/closing-issues-using-keywords).

     > Наприклад: `Closes#123` закриватиме завдання 123

5. Вкажіть, чи ви проводили тести на локальній копії сайту.

   - Це надзвичайно важливо при внесенні змін, які не стосуються зміни тексту (наприклад, документації чи опису завдань). До змін, яким потрібне локальне тестування, входять JavaScript, CSS або HTML (тобто ті, які можуть змінити функціональність чи макет сторінки).

   - Якщо ваш PR впливає на поведінку сторінки, він повинен супроводжуватися [інтеграційними тестами Cypress](how-to-add-cypress-tests.md).

## Feedback on Pull Requests

> :tada: Вітаємо зі створенням PR та дуже дякуємо, що знайшли час зробити свій внесок.

Наші модератори все переглянуть та залишать свій відгук. Будь ласка, наберіться терпіння та поважайте їхній час. Усі запити на злиття розглядаються за усталеним порядком.

І як завжди, не соромтесь ставити запитання [на форумі у категорії «Contributors»](https://forum.freecodecamp.org/c/contributors) або [у чаті](https://discord.gg/PRyKn3Vbay).

> [!TIP] Якщо ви хочете внести ще більше PR, ми рекомендуємо прочитати про [внесення змін та синхронізацію](how-to-setup-freecodecamp-locally.md#making-changes-locally), щоб уникнути видалення вашого форку.

## Conflicts on a Pull Request

Конфлікти можуть виникнути, якщо над репозиторієм працює багато помічників. Зміни можуть вплинути на PR, який очікує на перегляд та злиття.

Зазвичай у перебазовуванні немає потреби, оскільки ми стискаємо всі коміти. Однак, якщо перебазовування потрібне, ось що потрібно робити.

### For Usual Bug Fixes and Features

Коли ви працюєте над звичайними помилками та функціональностями на нашій гілці розробки `main`, ви можете виконати просте перебазовування:

1. Перебазуйте свою локальну копію:

   ```console
   git checkout <pr-branch>
   git pull --rebase upstream main
   ```

2. Вирішіть будь-які конфлікти та додайте/редагуйте коміти

   ```console
   # Або
   git add .
   git commit -m "chore: resolve conflicts"

   # Або
   git add .
   git commit --amend --no-edit
   ```

3. Відправте зміни до PR

   ```console
   git push --force origin <pr-branch>
   ```

### For Upcoming Curriculum and Features

Коли ви працюєте над функціональностями для майбутньої навчальної програми на гілках `next-*`, потрібно виконати команду cherry pick:

1. Переконайтесь, що віддалена гілка синхронізована з локальною:

   ```console
   git checkout main
   git fetch --all --prune
   git checkout next-python-projects
   git reset --hard upstream/next-python-projects
   ```

2. Зробіть резервну копію

   a. Або видаліть локальну гілку після створення резервної копії (якщо вона досі існує локально):

   ```console
   git checkout <pr-branch-name>

   # приклад:
   # git checkout feat/add-numpy-video-question

   git checkout -b <backup-branch-name>

   # приклад:
   #  git checkout -b backup-feat/add-numpy-video-question

   git branch -D <pr-branch-name>
   ```

   b. Або зробіть резервну копію гілки PR (якщо вона не існує локально):

   ```console
   git checkout -b <backup-branch-name> origin/<pr-branch-name>

   # приклад:
   #  git checkout -b backup-feat/add-numpy-video-question origin/feat/add-numpy-video-question
   ```

3. Розпочніть з нуля:

   ```console
   git checkout -b <pr-branch-name> next-python-projects
   git cherry-pick <commit-hash>
   ```

4. Розв’яжіть будь-які конфлікти, поприбирайте, встановіть залежності та запустіть тести

   ```console
   pnpm run clean

   pnpm install
   FCC_SUPERBLOCK='<superblock-name>' pnpm run test:curriculum 

   # приклад:

   # FCC_SUPERBLOCK='python-for-everybody' pnpm run test:curriculum

   ```

5. Якщо все виглядає добре, передайте до PR

   ```console
   git push --force origin <pr-branch-name>
   ```
