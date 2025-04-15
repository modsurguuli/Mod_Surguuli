<!DOCTYPE html>
<html lang="mn">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Мод Сургууль - Мастер Курс & Худалдаа</title>
  <style>
    body { font-family: Arial, sans-serif; margin: 0; background: #f4f9f4; color: #333; }
    header, footer { background: #2e7d32; color: white; text-align: center; padding: 1rem; }
    nav { background: #388e3c; display: flex; justify-content: center; flex-wrap: wrap; }
    nav a { color: white; text-decoration: none; margin: 10px; font-weight: bold; }
    .hero {
      background: url('https://images.unsplash.com/photo-1506765515384-028b60a970df') center/cover no-repeat;
      height: 250px; display: flex; align-items: center; justify-content: center;
      color: white; text-shadow: 1px 1px 3px rgba(0,0,0,0.7); text-align: center; padding: 1rem;
    }
    section { padding: 2rem 1rem; max-width: 1000px; margin: auto; }
    .tree-gallery { display: flex; flex-wrap: wrap; justify-content: center; gap: 1rem; margin-top: 2rem; }
    .tree-card { width: 280px; background: #fff; padding: 1rem; border-radius: 8px; box-shadow: 0 2px 6px rgba(0,0,0,0.1); text-align: center; }
    .tree-card img { width: 100%; height: 180px; object-fit: cover; border-radius: 6px; }
    .pagination { text-align: center; margin-top: 2rem; animation: flipIn 0.6s ease-in-out; }
    .pagination span { display: inline-block; margin: 0 5px; padding: 8px 14px; background: #ccc; border-radius: 50%; cursor: pointer; }
    .pagination span.active { background: #2e7d32; color: white; }
    @keyframes flipIn {
      from { transform: rotateY(90deg); opacity: 0; }
      to { transform: rotateY(0deg); opacity: 1; }
    }
    iframe { width: 100%; max-width: 100%; height: 700px; border: none; }
    @media (max-width: 768px) {
      nav { flex-direction: column; }
      .tree-card { width: 100%; }
      iframe { height: 500px; }
    }
  </style>
</head>
<body>
<header>
  <h1>Мод Сургууль</h1>
  <p>Мод үржүүлэг, тарилт, арчилгааны цахим сургалт</p>
</header>
<nav>
  <a href="#hero">Нүүр хуудас</a>
  <a href="#about">Танилцуулга</a>
  <a href="#courses">Сургалт</a>
  <a href="#trees">Худалдаа</a>
  <a href="#contact">Холбоо барих</a>
</nav>
<section id="hero" class="hero">
  <h2>Байгальд ээлтэй Мастер Курс: Үрээс ой хүртэл! 🌱</h2>
</section>

<section id="about">
  <h2>🟢 Танилцуулга</h2>
  <p>“Мод Сургууль” бол байгальд ээлтэй, тогтвортой ирээдүйг бүтээхэд чиглэсэн цахим сургалтын платформ юм. Манай сургалтууд нь ойн инженерүүдийн боловсруулсан, онол-практикийг хослуулсан агуулгатай.</p>
</section>

<section id="courses">
  <h2>🎓 Сургалтын агуулга</h2>
  <ul>
    <li><strong>1. Үрийн танилцуулга:</strong> Үрийн төрөл, хэлбэр, чанарын шалгуур</li>
    <li><strong>2. Үр бэлтгэх:</strong> Ариутгал, хөрс сонголт, сав баглаа</li>
    <li><strong>3. Үр тарих техник:</strong> Гүн, зай, усалгаа, хүлэмжний нөхцөл</li>
    <li><strong>4. Арчилгаа:</strong> Сүүдрэвч, тэжээл, өвчнөөс хамгаалалт</li>
    <li><strong>5. Тарилтын дараа:</strong> Амьдралтын хувь, дахин нөхөн тарих</li>
  </ul>
  <div style="text-align:center;">
    <iframe src="https://docs.google.com/forms/d/e/1FAIpQLScd_xxxxxxxxxxxxxx/viewform?embedded=true" width="100%" height="800" frameborder="0" marginheight="0" marginwidth="0">Түр хүлээнэ үү…</iframe>
    <p style="margin-top:1rem;"><strong>Сургалтын төлбөр: </strong>Голомт банк - Оренжэри Ган ХХК - <b>MN75 0015 00 6205150721</b></p>
  </div>
</section>

<section id="trees">
  <h2>🌳 Худалдаа - Модны үнийн санал</h2>
  <table style="width:100%; border-collapse:collapse;">
    <thead style="background:#2e7d32; color:white;">
      <tr>
        <th>Монгол нэр</th>
        <th>Латин нэр</th>
        <th>Өндөр</th>
        <th>Үнэ (₮)</th>
        <th>Тоо ширхэг</th>
        <th>Тооцоолсон үнэ</th>
      </tr>
    </thead>
    <tbody id="treeTable">
      <tr>
        <td>Хайлаас</td>
        <td>Ulmus pumila</td>
        <td>0.8–1.5 м</td>
        <td>2500</td>
        <td><input type="number" value="0" min="0" onchange="calculateTotal(this)"></td>
        <td class="total">0₮</td>
      </tr>
      <tr>
        <td>Шар хуайс</td>
        <td>Robinia pseudoacacia</td>
        <td>1.0–1.5 м</td>
        <td>3200</td>
        <td><input type="number" value="0" min="0" onchange="calculateTotal(this)"></td>
        <td class="total">0₮</td>
      </tr>
      <tr>
        <td>Гацуур</td>
        <td>Picea obovata</td>
        <td>1.3–1.5 м</td>
        <td>250000</td>
        <td><input type="number" value="0" min="0" onchange="calculateTotal(this)"></td>
        <td class="total">0₮</td>
      </tr>
      <tr>
  <td>Нарс</td>
  <td>Pinus sylvestris</td>
  <td>2.5–3.0 м</td>
  <td>350000</td>
  <td><input type="number" value="0" min="0" onchange="calculateTotal(this)"></td>
  <td class="total">0₮</td>
</tr>
<tr>
  <td>Хус</td>
  <td>Betula platyphylla</td>
  <td>2.0–3.0 м</td>
  <td>250000</td>
  <td><input type="number" value="0" min="0" onchange="calculateTotal(this)"></td>
  <td class="total">0₮</td>
</tr>
<tr>
  <td>Шинэс</td>
  <td>Larix sibirica</td>
  <td>2.2–2.5 м</td>
  <td>200000</td>
  <td><input type="number" value="0" min="0" onchange="calculateTotal(this)"></td>
  <td class="total">0₮</td>
</tr>
<tr>
  <td>Голт бор</td>
  <td>Spiraea media</td>
  <td>1.3–1.5 м</td>
  <td>15000</td>
  <td><input type="number" value="0" min="0" onchange="calculateTotal(this)"></td>
  <td class="total">0₮</td>
</tr>
<tr>
  <td>Хар интоор</td>
  <td>Prunus padus</td>
  <td>0.3–0.5 м</td>
  <td>10500</td>
  <td><input type="number" value="0" min="0" onchange="calculateTotal(this)"></td>
  <td class="total">0₮</td>
</tr>
<tr>
  <td>Үхрийн нүд</td>
  <td>Ribes nigrum</td>
  <td>0.3–0.6 м</td>
  <td>15000</td>
  <td><input type="number" value="0" min="0" onchange="calculateTotal(this)"></td>
  <td class="total">0₮</td>
</tr>
<tr>
  <td>Чацаргана</td>
  <td>Hippophae rhamnoides</td>
  <td>1.0–1.2 м</td>
  <td>2500</td>
  <td><input type="number" value="0" min="0" onchange="calculateTotal(this)"></td>
  <td class="total">0₮</td>
</tr>
<tr>
  <td>Улиас</td>
  <td>Populus suaveolens</td>
  <td>1.6–2.0 м</td>
  <td>8500</td>
  <td><input type="number" value="0" min="0" onchange="calculateTotal(this)"></td>
  <td class="total">0₮</td>
</tr>
<tr>
  <td>Бургас</td>
  <td>Salix caprea</td>
  <td>1.6–2.0 м</td>
  <td>2500</td>
  <td><input type="number" value="0" min="0" onchange="calculateTotal(this)"></td>
  <td class="total">0₮</td>
</tr>
<tr>
  <td>Өрөл</td>
  <td>Berberis sibirica</td>
  <td>0.5–0.8 м</td>
  <td>8500</td>
  <td><input type="number" value="0" min="0" onchange="calculateTotal(this)"></td>
  <td class="total">0₮</td>
</tr>
<tr>
  <td>Сарнай</td>
  <td>Rosa rugosa</td>
  <td>0.3–0.5 м</td>
  <td>35000</td>
  <td><input type="number" value="0" min="0" onchange="calculateTotal(this)"></td>
  <td class="total">0₮</td>
</tr>
<tr>
  <td>Агч</td>
  <td>Acer ginnala</td>
  <td>1.2–1.5 м</td>
  <td>3500</td>
  <td><input type="number" value="0" min="0" onchange="calculateTotal(this)"></td>
  <td class="total">0₮</td>
</tr>
    </tbody>
  </table>
  <p style="text-align:center; margin-top:1rem;"><strong>💡 Урамшуулал:</strong> 100 ширхэгээс дээш -2%, 1000 ширхэгээс дээш -5%</p>
</section>
<script>
function calculateTotal(input) {
  const row = input.parentElement.parentElement;
  const price = parseInt(row.children[3].textContent);
  const qty = parseInt(input.value);
  let discount = 0;
  if (qty >= 1000) discount = 0.05;
  else if (qty >= 100) discount = 0.02;
  const total = qty * price * (1 - discount);
  row.querySelector('.total').textContent = total.toLocaleString() + '₮';
}
</script>

<section id="contact">
  <h2>📞 Холбоо барих</h2>
  <p>Бидэнтэй холбогдохын тулд дараах мэдээллийг ашиглана уу:</p>
  <ul>
    <li>📍 Хаяг: Улаанбаатар хот, Хан-Уул дүүрэг, 52-р байр</li>
    <li>📞 Утас: +976 7211-1311, 8045-6899</li>
    <li>📧 Имэйл: modsurguuli@gmail.com</li>
  </ul>
</section>

<footer>
  &copy; 2025 Мод Сургууль — Урамшуулалт мод захиалга. Бүх эрх хуулиар хамгаалагдсан.
</footer>
</body>
</html>
