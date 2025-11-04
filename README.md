<!DOCTYPE html>
<html lang="ru">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">

<title>Устав семьи BUDKEVSKY</title>

<style>
  body {
    margin: 0;
    font-family: sans-serif;
    background: #371A94;
    color: #FFFFFF;
  }

  header {
    background: rgba(255,255,255,0.15);
    padding: 20px;
    text-align: center;
    border-bottom: 2px solid #5A0B76;
  }

  .logo {
    width: 140px;
    max-width: 60%;
    border-radius: 8px;
  }

  h1 {
    margin: 10px 0 0;
    font-size: 28px;
  }

  main {
    max-width: 900px;
    padding: 20px;
    margin: 20px auto;
    font-size: 18px;
    line-height: 1.6;
  }

  ol.nested {
    counter-reset: section;
    list-style: none;
    padding-left: 0;
  }

  ol.nested > li {
    counter-increment: section;
    margin-bottom: 15px;
  }

  ol.nested > li:before {
    content: counter(section) ". ";
    font-weight: bold;
  }

  ol.nested li ol {
    counter-reset: subsection;
    margin-left: 20px;
    list-style: none;
  }

  ol.nested li ol li {
    counter-increment: subsection;
  }

  ol.nested li ol li:before {
    content: counter(section) "." counter(subsection) ". ";
  }

  /* ✅ Адаптив */
  @media (max-width: 600px) {
    h1 {
      font-size: 22px;
    }
    main {
      padding: 15px;
      font-size: 16px;
    }
    .logo {
      width: 120px;
    }
  }
</style>
</head>

<body>
<header>
  <img class="logo" src="" alt="Логотип">
  <h1>06 сервер</h1>
  <h1>Устав семьи Будевских</h1>
</header>

<main>
  <ol class="nested">
    <li>Основные положения
      <ol>
        <li>Каждый член семьи обязан знать устав.</li>
        <li>Незнание устава не освобождает от ответственности.
          Нарушение устава влечёт наказание:
          <ul>
            <li>Выговор</li>
            <li>Устный разговор</li>
            <li>Понижение</li>
            <li>Исключение из семьи с занесением в ЧС (по решению главного следящего или лидера)</li>
          </ul>
        </li>
      </ol>
    </li>

    <li>Дисциплина и обязанности
      <ol>
        <li>Участники обязаны проявлять уважение к членам семьи и игрокам.</li>
        <li>Запрещены оскорбления, мат, провокации.</li>
        <li>Заместитель обязан быть примером и помогать игрокам.</li>
      </ol>
    </li>

    <li>Общение
      <ol>
        <li>Общение должно быть спокойным и конструктивным.</li>
        <li>Запрещены мат, агрессия, провокации.</li>
      </ol>
    </li>

    <li>Участие в жизни семьи
      <ol>
        <li>Каждый обязан участвовать в развитии семьи и помогать новичкам.</li>
      </ol>
    </li>

    <li>Конфиденциальность
      <ol>
        <li>Запрещено разглашать личные данные участников.</li>
      </ol>
    </li>

    <li>Поддержка
      <ol>
        <li>Старшие обязаны помогать и обучать новичков.</li>
      </ol>
    </li>
  </ol>
</main>
</body>
</html>>
