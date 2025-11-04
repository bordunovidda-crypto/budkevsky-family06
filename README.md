<html lang="ru">
<head>
<meta charset="UTF-8">
<title>BUDKEVSKY — Главная</title>

<style>
  body {
    margin: 0;
    font-family: sans-serif;
    background: #371A94;
    color: #FFFFFF;
  }

  header {
    background: rgba(255,255,255,0.1);
    padding: 20px;
    text-align: center;
    border-bottom: 2px solid #371A94;
  }

  .logo {
    width: 120px;
    filter: brightness(0) saturate(100%) invert(17%) sepia(27%) 
            saturate(2887%) hue-rotate(245deg) brightness(85%) contrast(90%);
  }

  .page {
    display: none;
    max-width: 900px;
    margin: 20px auto;
    padding: 20px;
  }

  .active {
    display: block;
  }

  button {
    margin-top: 15px;
    padding: 10px 18px;
    border: none;
    cursor: pointer;
    border-radius: 8px;
    font-weight: bold;
  }

  .btn-nav {
    background: rgba(255,255,255,0.18);
    color: #FFFFFF;
    margin: 10px;
  }

  .btn-nav:hover {
    background: rgba(255,255,255,0.3);
  }

  h2 {
    color: #FFFFFF;
    border-bottom: 1px solid rgba(255,255,255,0.25);
    padding-bottom: 6px;
  }

  /* Нумерация устава */
  ol.nested {
    counter-reset: section;
    list-style: none;
    padding-left: 0;
  }
  ol.nested > li {
    counter-increment: section;
    margin-bottom: 15px;
  }
  ol.nested > li::before {
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
  ol.nested li ol li::before {
    content: counter(section) "." counter(subsection) ". ";
  }
</style>
</head>
<body>

<header>
  <img class="logo" src="https://i.postimg.cc/6QWrj9Nq/IMG-0302.png" alt="Логотип">
  <h1>Семья Budkevsky</h1>
</header>

<!-- ================== ГЛАВНАЯ ================== -->
<div id="home" class="page active">
  <h2>Главное меню</h2>

  <button class="btn-nav" onclick="openPage('ustav')">Устав семьи</button>
  <button class="btn-nav" onclick="openPage('ceny')">Цены на ранги</button>
</div>

<!-- ================== УСТАВ ================== -->
<div id="ustav" class="page">
  <h2>Устав семьи</h2>

  <ol class="nested">
    <li>Основные положения
      <ol>
        <li>Каждый член семьи обязан знать устав.</li>
        <li>Незнание устава не освобождает от ответственности. Нарушение устава влечёт наказание:
          <ul>
            Выговор,
            устный разговор,
            понижение,
            исключение из семьи с занесением в ЧС (на рассмотрение главного следящего или лидера семьи).
          </ul>
        </li>
      </ol>
    </li>

    <li>Дисциплина и обязанности
      <ol>
        <li>Участники обязаны проявлять уважение к другим членам семьи и игрокам.</li>
        <li>Запрещено использование нецензурной брани, оскорблений и провокаций.</li>
        <li>Заместитель семьи — образец поведения.</li>
      </ol>
    </li>

    <li>Общение
      <ol>
        <li>Общение должно быть уважительным и конструктивным.</li>
        <li>Запрещён мат и агрессия.</li>
      </ol>
    </li>

    <li>Участие в жизни семьи
      <ol>
        <li>Каждый обязан помогать новичкам.</li>
      </ol>
    </li>

    <li>Конфиденциальность
      <ol>
        <li>Нельзя передавать личную информацию.</li>
      </ol>
    </li>

    <li>Поддержка и помощь
      <ol>
        <li>Опытные участники помогают новичкам.</li>
      </ol>
    </li>
  </ol>

  <button class="btn-nav" onclick="openPage('home')">Назад</button>
</div>

<!-- ================== ЦЕНЫ ================== -->
<div id="ceny" class="page">
  <h2>Цены на ранги</h2>

  <p>2 — <b>45 000 ₽</b></p>
  <p>3 — <b>75 000 ₽</b></p>
  <p>4 — <b>100 000 ₽</b></p>
  <p>5 — <b>125 000 ₽</b></p>
  <p>6 (стрелок) — <b>1 000 000 ₽</b> или доверка</p>

  <button class="btn-nav" onclick="openPage('home')">Назад</button>
</div>

<script>
  function openPage(name) {
    document.querySelectorAll('.page')
      .forEach(p => p.classList.remove('active'));
    document.getElementById(name).classList.add('active');
  }
</script>

</body>
</html>
