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
    .course, .tree { background: white; padding: 1rem; margin: 1rem 0; border-radius: 8px; box-shadow: 0 1px 4px rgba(0,0,0,0.1); }
    .tree img { width: 100%; max-width: 200px; float: left; margin-right: 1rem; border-radius: 4px; }
    .tree-content { overflow: hidden; }
    iframe { width: 100%; height: 700px; border: none; margin-top: 2rem; }
    .price-input { width: 80px; padding: 5px; }
    .price-result { font-weight: bold; margin-top: 10px; display: block; }
    @media (max-width: 768px) {
      nav { flex-direction: column; }
      .tree img { float: none; margin: auto auto 1rem auto; display: block; }
      iframe { height: 900px; }
    }
  </style>
  <script>
    function calculatePrice(priceId, qtyId, outputId) {
      const unitPrice = parseInt(document.getElementById(priceId).value);
      const qty = parseInt(document.getElementById(qtyId).value);
      let discount = 0;
      if (qty >= 1000) discount = 0.05;
      else if (qty >= 100) discount = 0.02;
      const total = qty * unitPrice * (1 - discount);
      document.getElementById(outputId).innerText = 'Нийт үнэ: ' + total.toLocaleString('mn-MN') + '₮ (' + (discount * 100) + '% хөнгөлөлттэй)';
    }
  </script>
</head>
<body>
  <header>
    <h1>Мод Сургууль</h1>
    <p>Мод үржүүлэг, тарилт, арчилгааны цахим сургалт</p>
  </header>

  <nav>
  <a href="#hero">Нүүр хуудас</a>
  <a href="#courses">Сургалт</a>
  <a href="#trees">Худалдаа</a>
</nav>

  <section id="hero" class="hero">
  <h2>Байгальд ээлтэй Мастер Курс: Үрээс ой хүртэл! 🌱</h2>
</section>

<section id="intro">
  <h2>🟢 Яагаад энэ сургалтад суух ёстой вэ?</h2>
  <p>
    Энэ сургалт нь мод үржүүлэг, тарилт, арчилгааны үндэс суурь мэдлэгийг богино хугацаанд, оновчтой аргаар олгоно. Байгальд ээлтэй, орлого бүтээх боломжтой энэхүү мэдлэг таны амьдралд бодит үр дүн авчрах болно.
  </p>
  <p style="text-align:center; margin-top: 1.5rem;">
    <a href="#order" style="background:#2e7d32; color:white; padding: 12px 24px; text-decoration: none; border-radius: 6px; font-weight: bold;">📥 Сургалтад бүртгүүлэх</a>
  </p>
</section>

  <section id="courses">
  <h2>🎓 Сургалтын блокууд</h2>
  <table style="width:100%; border-collapse: collapse;">
    <thead>
      <tr style="background-color:#c8e6c9;">
        <th style="padding: 10px; border: 1px solid #ccc; text-align:left;">Сэдэв</th>
        <th style="padding: 10px; border: 1px solid #ccc; text-align:left;">Дотоод хичээлүүд</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td style="padding: 10px; border: 1px solid #ccc;">1. Үрийн танилцуулга</td>
        <td style="padding: 10px; border: 1px solid #ccc;">Үрийн төрөл, хэлбэр, чанарын шалгуур</td>
      </tr>
      <tr>
        <td style="padding: 10px; border: 1px solid #ccc;">2. Үр бэлтгэх</td>
        <td style="padding: 10px; border: 1px solid #ccc;">Ариутгал, хөрс сонголт, сав баглаа</td>
      </tr>
      <tr>
        <td style="padding: 10px; border: 1px solid #ccc;">3. Үр тарих техник</td>
        <td style="padding: 10px; border: 1px solid #ccc;">Гүн, зай, усалгаа, хүлэмжний нөхцөл</td>
      </tr>
      <tr>
        <td style="padding: 10px; border: 1px solid #ccc;">4. Арчилгаа</td>
        <td style="padding: 10px; border: 1px solid #ccc;">Сүүдрэвч, тэжээл, өвчнөөс хамгаалалт</td>
      </tr>
      <tr>
        <td style="padding: 10px; border: 1px solid #ccc;">5. Тарилтын дараа</td>
        <td style="padding: 10px; border: 1px solid #ccc;">Амьдралтын хувь, дахин нөхөн тарих</td>
      </tr>
    </tbody>
  </table>
</section>

<section id="course-detail">
  <h2>📚 Хичээлийн агуулга (Тайлбар)</h2>
  <p>
    Энэхүү мастер курс нь үрийн төрөл, хэлбэр, чанарын үнэлгээ зэргээс эхэлж, хөрс болон сав баглаа сонголт, ариутгалын аргад суурилсан үр бэлтгэлд гүнзгий орно. Цаашлаад үрийг хэрхэн тохирсон гүнд, зөв зайнд суулгах, хүлэмж болон байгалийн нөхцөлд ургуулах практик мэдлэгийг эзэмшүүлнэ.
  </p>
  <p>
    Мөн арчилгааны үе шат бүрд шаардлагатай сүүдрэвч, тэжээл, усалгаа, ургамлын хамгаалалт зэрэг мэргэжлийн аргуудыг заана. Сургалтын төгсгөлд модны амьдралтын хувь, нөхөн суулгалтын ач холбогдлыг онцолж, байгальд ээлтэй урт хугацааны арчилгааны талаар чиглүүлнэ.
  </p>
</section>

<section id="trees">
  <h2>🌳 Худалдаалж буй мод (Үнийн санал, хөнгөлөлт)</h2>
  <p>
    Манай мод үржүүлгийн талбайгаас дараах 26 төрлийн мод, бут сөөгийг захиалан худалдан авах боломжтой. Бүх модны үнэ нь өндөр, нас, чанарын ангиллаар ялгаатай бөгөөд 100 ширхэгээс дээш тохиолдолд 2%, 1000 ширхэгээс дээш бол 5% хөнгөлөлт тооцогдоно.
  </p>
  <table style="width:100%; border-collapse: collapse; margin-top: 1rem;">
    <thead>
      <tr style="background-color:#c8e6c9;">
        <th style="padding: 10px; border: 1px solid #ccc;">Монгол нэр</th>
        <th style="padding: 10px; border: 1px solid #ccc;">Латин нэр</th>
        <th style="padding: 10px; border: 1px solid #ccc;">Өндөр</th>
        <th style="padding: 10px; border: 1px solid #ccc;">Үнэ (₮)</th>
      </tr>
    </thead>
    <tbody>
      <tr><td>Хайлаас</td><td>Ulmus pumila</td><td>0.8–1.5 м</td><td>1,800–2,500₮</td></tr>
      <tr><td>Шар хуайс</td><td>Robinia pseudoacacia</td><td>1.0–1.5 м</td><td>2,500–3,200₮</td></tr>
      <tr><td>Гацуур</td><td>Picea obovata</td><td>1.0–2.0 м</td><td>220,000–350,000₮</td></tr>
      <tr><td>Нарс</td><td>Pinus sylvestris</td><td>1.5–3.0 м</td><td>250,000–350,000₮</td></tr>
      <tr><td>Хус</td><td>Betula platyphylla</td><td>2.0–3.0 м</td><td>250,000₮</td></tr>
      <tr><td>Шинэс</td><td>Larix sibirica</td><td>0.8–2.5 м</td><td>55,000–200,000₮</td></tr>
      <tr><td>Голт бор</td><td>Spiraea media</td><td>1.0–1.5 м</td><td>10,500–15,000₮</td></tr>
      <tr><td>Хар интоор</td><td>Prunus padus</td><td>0.3–0.5 м</td><td>10,500₮</td></tr>
      <tr><td>Үхрийн нүд</td><td>Ribes nigrum</td><td>0.3–0.6 м</td><td>15,000₮</td></tr>
      <tr><td>Чацаргана</td><td>Hippophae rhamnoides</td><td>0.6–1.2 м</td><td>2,200–2,500₮</td></tr>
      <tr><td>Улиас</td><td>Populus suaveolens</td><td>1.0–2.0 м</td><td>4,500–8,500₮</td></tr>
      <tr><td>Бургас</td><td>Salix babylonica</td><td>1.2–2.0 м</td><td>2,200–2,500₮</td></tr>
      <tr><td>Өрөл</td><td>Berberis sibirica</td><td>0.5–0.8 м</td><td>8,500₮</td></tr>
      <tr><td>Сарнай</td><td>Rosa rugosa</td><td>0.3–0.5 м</td><td>35,000₮</td></tr>
      <tr><td>Агч</td><td>Acer ginnala</td><td>1.2–1.5 м</td><td>3,500₮</td></tr>
      <tr><td>Нохой хошуу</td><td>Rosa davurica</td><td>0.5–1.0 м</td><td>12,000₮</td></tr>
<tr><td>Гацуур (том)</td><td>Picea obovata</td><td>2.5–3.0 м</td><td>400,000₮</td></tr>
<tr><td>Нарс (том)</td><td>Pinus sylvestris</td><td>3.0–4.0 м</td><td>450,000₮</td></tr>
<tr><td>Хуш</td><td>Pinus sibirica</td><td>1.0–2.0 м</td><td>380,000₮</td></tr>
<tr><td>Гүйлс</td><td>Prunus armeniaca</td><td>1.0–1.5 м</td><td>25,000₮</td></tr>
<tr><td>Тошлой</td><td>Ribes uva-crispa</td><td>0.5–1.0 м</td><td>15,000₮</td></tr>
<tr><td>Чацаргана (эм)</td><td>Hippophae rhamnoides</td><td>0.8–1.0 м</td><td>2,500₮</td></tr>
<tr><td>Чацаргана (эрэгтэй)</td><td>Hippophae rhamnoides</td><td>0.8–1.0 м</td><td>2,000₮</td></tr>
<tr><td>Цагаан бургас</td><td>Salix alba</td><td>2.0–3.0 м</td><td>3,500₮</td></tr>
<tr><td>Ногоон улиас</td><td>Populus laurifolia</td><td>2.0–3.0 м</td><td>6,500₮</td></tr>
<tr><td>Монгол улиас</td><td>Populus davidiana</td><td>1.5–2.0 м</td><td>4,800₮</td></tr>
    </tbody>
  </table>
  <p style="margin-top: 1rem;">
    ➕ 100 ширхэгээс дээш худалдан авалт хийсэн тохиолдолд нийт дүнгээс 2%, харин 1000 ширхэгээс дээш бол 5% хөнгөлөлт автомат тооцогдоно. Захиалгаа доорх холбоо барих хэсэгт өгнө үү.
  </p>
</section>



<section id="contact">
  <h2>📞 Холбоо барих</h2>
  <p><strong>Имэйл:</strong> modsurguuli@gmail.com</p>
  <p><strong>Утас:</strong> 7211-1311, 8045-6899</p>
  <p><strong>Байршил:</strong> Улаанбаатар хот, Хан-Уул дүүрэг, 52-р байр</p>
</section>

<footer>
  &copy; 2025 Мод Сургууль. Бүх эрх хуулиар хамгаалагдсан.
</footer>
</body>
</html>
