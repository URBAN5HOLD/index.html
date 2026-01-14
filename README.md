<!DOCTYPE html>
<html lang="ar">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>الموقع الرسمي للمنتجات</title>

<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@500;600&family=Inter:wght@300;400&display=swap" rel="stylesheet">

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: 'Inter', sans-serif;
  background: linear-gradient(180deg, rgba(30,20,10,0.95), rgba(245,240,230,0.95));
  color: #111;
  min-height: 100vh;
  padding: 40px 20px;
}

/* عنوان الموقع */
.brand {
  font-family: 'Playfair Display', serif;
  font-size: 36px;
  color: #fff;
  text-align: center;
  margin-bottom: 10px;
}

.subtitle {
  text-align: center;
  color: #e8dccb;
  font-size: 16px;
  margin-bottom: 40px;
}

/* container للبطاقات */
.product-container {
  display: flex;
  flex-direction: column;
  gap: 25px;
  align-items: center;
}

/* البطاقة الرئيسية */
.product-main {
  background: rgba(255,255,255,0.12); /* glass effect */
  backdrop-filter: blur(10px);
  border-radius: 25px;
  width: 90%;
  max-width: 600px;
  padding: 30px;
  box-shadow: 0 25px 60px rgba(0,0,0,0.35);
  cursor: pointer;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
}

.product-main:hover {
  transform: translateY(-8px);
  box-shadow: 0 30px 80px rgba(0,0,0,0.4);
}

.product-main img {
  width: 100%;
  max-width: 400px;
  border-radius: 20px;
  margin-bottom: 20px;
  transition: transform 0.3s ease;
}

.product-main:hover img {
  transform: scale(1.05);
}

.product-main .title {
  font-family: 'Playfair Display', serif;
  font-size: 28px;
  margin-bottom: 15px;
}

.product-main .desc {
  font-size: 16px;
  color: #eee;
  margin-bottom: 20px;
  line-height: 1.6;
}

.product-main .features {
  list-style: none;
  margin-bottom: 20px;
}

.product-main .features li {
  font-size: 15px;
  margin-bottom: 6px;
}

.product-main .price {
  font-size: 22px;
  font-weight: 600;
  margin-bottom: 20px;
}

.product-main .btn {
  background: linear-gradient(135deg, #25D366, #1ebe5d);
  color: #fff;
  text-decoration: none;
  padding: 14px 0;
  border-radius: 14px;
  font-size: 17px;
  font-weight: bold;
  width: 80%;
  transition: background 0.3s ease;
}

.product-main .btn:hover {
  background: linear-gradient(135deg, #1ebe5d, #25D366);
}

/* الصف ديال البطاقات الصغرى */
.product-row {
  display: flex;
  gap: 25px;
  flex-wrap: wrap;
  justify-content: center;
  width: 100%;
}

.product-card {
  background: rgba(255,255,255,0.12);
  backdrop-filter: blur(8px);
  border-radius: 20px;
  width: 250px;
  padding: 20px;
  box-shadow: 0 20px 50px rgba(0,0,0,0.3);
  cursor: pointer;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
  text-align: center;
}

.product-card:hover {
  transform: translateY(-6px);
  box-shadow: 0 25px 70px rgba(0,0,0,0.35);
}

.product-card img {
  width: 100%;
  border-radius: 15px;
  margin-bottom: 15px;
  transition: transform 0.3s ease;
}

.product-card:hover img {
  transform: scale(1.05);
}

.product-card .title {
  font-family: 'Playfair Display', serif;
  font-size: 20px;
  margin-bottom: 10px;
}

.product-card .desc {
  font-size: 14px;
  color: #eee;
  margin-bottom: 15px;
}

.product-card .features {
  list-style: none;
  margin-bottom: 15px;
}

.product-card .features li {
  font-size: 13px;
  margin-bottom: 5px;
}

.product-card .price {
  font-size: 18px;
  font-weight: 600;
  margin-bottom: 15px;
}

.product-card .btn {
  background: linear-gradient(135deg, #25D366, #1ebe5d);
  color: #fff;
  text-decoration: none;
  padding: 12px 0;
  border-radius: 12px;
  font-size: 15px;
  font-weight: bold;
  transition: background 0.3s ease;
}

.product-card .btn:hover {
  background: linear-gradient(135deg, #1ebe5d, #25D366);
}

/* responsive */
@media(max-width:900px){
  .product-row {
    flex-direction: column;
    align-items: center;
  }

  .product-main {
    width: 95%;
  }
}

</style>
</head>
<body>

<div class="container">

  <div class="brand">Brand Officiel</div>
  <div class="subtitle">منتجات راقية، تجربة مثالية.</div>

  <div class="product-container">
    
    <!-- البطاقة الرئيسية -->
    <a href="https://wa.me/212691444558?text=سلام، بغيت نطلب الجل" target="_blank" class="product-main">
      <img src="gel.jpg" alt="جيل الشعر">
      <div class="title">جيل تثبيت الشعر</div>
      <div class="desc">
        جل قوي لتثبيت الشعر، يعطي لمعة طبيعية ويترك شعرك ثابت طوال اليوم بدون قساوة.
      </div>
      <ul class="features">
        <li>✔ ثبات قوي</li>
        <li>✔ ملمس طبيعي</li>
        <li>✔ مناسب للاستخدام اليومي</li>
      </ul>
      <div class="price">35 درهم</div>
      <div class="btn">اطلب الآن عبر واتساب</div>
    </a>

    <!-- الصف ديال البطاقات الصغرى -->
    <div class="product-row">
      <!-- المنتج الثاني -->
      <a href="https://wa.me/212691444558?text=سلام، بغيت نطلب سبراي" target="_blank" class="product-card">
        <img src="spray.jpg" alt="سبراي الشعر">
        <div class="title">سبراي تثبيت الشعر</div>
        <div class="desc">سبراي خفيف يعطي ثبات متوسط ولمسة ناعمة مع حماية من الرطوبة.</div>
        <ul class="features">
          <li>✔ ثبات متوسط</li>
          <li>✔ حماية من الرطوبة</li>
          <li>✔ مثالي للشعر القصير والطويل</li>
        </ul>
        <div class="price">40 درهم</div>
        <div class="btn">اطلب الآن عبر واتساب</div>
      </a>

      <!-- المنتج الثالث -->
      <a href="https://wa.me/212691444558?text=سلام، بغيت نطلب واكس" target="_blank" class="product-card">
        <img src="wax.jpg" alt="واكس الشعر">
        <div class="title">واكس الشعر</div>
        <div class="desc">واكس غني لتشكيل الشعر بسهولة ولمسة نهائية لامعة طبيعية.</div>
        <ul class="features">
          <li>✔ تشكيل سهل ومرن</li>
          <li>✔ لمسة لامعة طبيعية</li>
          <li>✔ مثالي للشعر القصير والطويل</li>
        </ul>
        <div class="price">45 درهم</div>
        <div class="btn">اطلب الآن عبر واتساب</div>
      </a>
    </div>

  </div>

</div>

</body>
</html>
