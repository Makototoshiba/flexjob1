<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8" />
  <title>FlexJob</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #f4f4f4;
      margin: 0;
      padding: 1rem;
    }
    header {
      text-align: center;
    }
    .description {
      margin: 1rem 0;
      padding: 1rem;
      background: #e0f0ff;
      border-left: 5px solid #007bff;
    }
    main {
      display: flex;
      flex-direction: row;
      gap: 1rem;
      flex-wrap: wrap;
    }
    section {
      background: white;
      padding: 1rem;
      flex: 1 1 48%;
      border: 1px solid #ccc;
      border-radius: 6px;
    }
    input, select, textarea {
      width: 100%;
      margin: 0.3rem 0;
      padding: 0.5rem;
      border: 1px solid #ccc;
      border-radius: 4px;
      box-sizing: border-box;
    }
    button {
      padding: 0.5rem 1rem;
      background: #007bff;
      border: none;
      color: white;
      cursor: pointer;
      border-radius: 4px;
    }
    button:hover {
      background: #0056b3;
    }
    .slot {
      padding: 0.5rem;
      border-bottom: 1px solid #ddd;
    }
  </style>
</head>
<body>
  <header>
    <h1>FlexJob</h1>
    <p>Работа на твоих условиях — быстро и удобно</p>
  </header>
  <section class="description">
    FlexJob — сервис для поиска временной работы и подработок. Работодатели размещают задания с датой, временем и оплатой, а работники выбирают и откликаются в пару кликов.
  </section>
  <main>
    <section id="employer-section">
      <h2>Добавить задание (Работодатель)</h2>
      <input type="text" id="title" placeholder="Название задания" />
      <input type="date" id="dateStart" />
      <select id="timeStart"></select>
      <input type="date" id="dateEnd" />
      <select id="timeEnd"></select>
      <input type="number" id="rate" placeholder="Оплата в час (₽)" />
      <textarea id="desc" placeholder="Описание задания"></textarea>
      <input type="text" id="contact" placeholder="Контакты" />
      <button id="addSlotBtn">Добавить</button>
    </section>
    <section id="worker-section">
      <h2>Найти задание (Работник)</h2>
      <input type="text" id="searchText" placeholder="Поиск по названию/описанию" />
      <input type="number" id="minRate" placeholder="Мин. ставка (₽)" />
      <input type="date" id="dateFrom" />
      <button id="filterBtn">Применить</button>
      <div id="slots"></div>
    </section>
  </main>
  <script>
    function fillTimeSelect(id) {
      const select = document.getElementById(id);
      for (let h = 0; h < 24; h++) {
        for (let m = 0; m < 60; m += 30) {
          const hh = h.toString().padStart(2, "0");
          const mm = m.toString().padStart(2, "0");
          const opt = document.createElement("option");
          opt.value = `${hh}:${mm}`;
          opt.text = `${hh}:${mm}`;
          select.appendChild(opt);
        }
      }
    }
    fillTimeSelect("timeStart");
    fillTimeSelect("timeEnd");

    let slots = [];

    function renderSlots() {
      const container = document.getElementById("slots");
      container.innerHTML = "";
      const search = document.getElementById("searchText").value.toLowerCase();
      const minRate = parseInt(document.getElementById("minRate").value) || 0;
      const dateFrom = document.getElementById("dateFrom").value;

      const filtered = slots.filter(
        (s) =>
          (!search ||
            s.title.toLowerCase().includes(search) ||
            s.desc.toLowerCase().includes(search)) &&
          s.rate >= minRate &&
          (!dateFrom || new Date(s.start) >= new Date(dateFrom))
      );

      if (filtered.length === 0) {
        container.innerHTML = "<p>Нет подходящих заданий</p>";
        return;
      }

      filtered.forEach((slot) => {
        const div = document.createElement("div");
        div.className = "slot";
        div.innerHTML = `
          <strong>${slot.title}</strong><br>
          ${slot.start} – ${slot.end}<br>
          ${slot.rate} ₽/час<br>
          ${slot.desc}<br>
          Контакты: ${slot.contact}
        `;
        container.appendChild(div);
      });
    }

    function addSlot() {
      const title = document.getElementById("title").value;
      const dateStart = document.getElementById("dateStart").value;
      const timeStart = document.getElementById("timeStart").value;
      const dateEnd = document.getElementById("dateEnd").value;
      const timeEnd = document.getElementById("timeEnd").value;
      const rate = parseInt(document.getElementById("rate").value);
      const desc = document.getElementById("desc").value;
      const contact = document.getElementById("contact").value;

      if (
        !title ||
        !dateStart ||
        !timeStart ||
        !dateEnd ||
        !timeEnd ||
        !rate ||
        !contact
      ) {
        alert("Заполните все поля");
        return;
      }

      const start = `${dateStart} ${timeStart}`;
      const end = `${dateEnd} ${timeEnd}`;
      slots.push({ title, start, end, rate, desc, contact });
      renderSlots();
    }

    document.getElementById("addSlotBtn").addEventListener("click", addSlot);
    document.getElementById("filterBtn").addEventListener("click", renderSlots);
  </script>
</body>
</html>
