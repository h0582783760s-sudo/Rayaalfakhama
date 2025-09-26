<!DOCTYPE html>
<html lang="ar">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>راية الفخامة لتأجير السيارات | Rayaalfakhama Rental Car</title>
<style>
  body {font-family: Arial, sans-serif; margin:0; padding:0; background-color: #f9f9f9; transition: all 0.3s ease;}
  header {background-color: #ff6600; color: white; padding: 20px; text-align: center; position: relative;}
  nav {display: flex; justify-content: center; gap: 20px; background-color: #333;}
  nav a {color: white; text-decoration: none; padding: 10px 15px;}
  nav a:hover {background-color: #ff6600; border-radius: 5px;}
  section {padding: 40px 20px; max-width: 1000px; margin: auto;}
  h2 {color: #ff6600;}
  .services, .contact, .gallery, .pricing {display: flex; flex-wrap: wrap; gap: 20px;}
  .service-box, .contact-box, .gallery img, .car-box {background-color: white; flex: 1 1 300px; padding: 20px; border-radius: 10px; box-shadow: 0 0 10px rgba(0,0,0,0.1);}
  .gallery img {padding: 0; cursor: pointer; object-fit: cover; height: 200px; width: 100%;}
  .car-box img {height:150px; width:100%; object-fit: cover; border-radius:10px; margin-bottom:10px;}
  button {background-color: #ff6600; color:white; border:none; padding:10px; border-radius:5px; cursor:pointer;}
  button:hover {opacity:0.9;}
  footer {background-color: #333; color: white; text-align:center; padding: 20px;}
  .lang-switch {position: absolute; top: 20px; right: 20px;}
  .lang-switch button {background: white; border: none; padding: 5px 10px; cursor: pointer; font-weight: bold; border-radius: 5px;}
  #lightbox {position: fixed; display: none; top:0; left:0; width:100%; height:100%; background: rgba(0,0,0,0.8); justify-content: center; align-items: center; z-index: 1000;}
  #lightbox img {max-width: 90%; max-height: 80%; border-radius: 10px;}
  form {display:flex; flex-direction:column; gap:10px; background:white; padding:20px; border-radius:10px; box-shadow:0 0 10px rgba(0,0,0,0.1);}
  input, select {padding:10px; border-radius:5px; border:1px solid #ccc;}
</style>
</head>
<body>

<header>
  <h1 id="title">راية الفخامة لتأجير السيارات</h1>
  <div class="lang-switch">
    <button onclick="switchLanguage('ar')">العربية</button>
    <button onclick="switchLanguage('en')">EN</button>
  </div>
</header>

<nav>
  <a href="#home" id="nav-home">الرئيسية</a>
  <a href="#about" id="nav-about">من نحن</a>
  <a href="#services" id="nav-services">خدماتنا</a>
  <a href="#pricing" id="nav-pricing">أسعار السيارات</a>
  <a href="#contact" id="nav-contact">تواصل معنا</a>
</nav>

<section id="home">
  <h2 id="home-title">مرحباً بكم في راية الفخامة</h2>
  <p id="home-text">شركة رائدة في تأجير السيارات في الإمارات العربية المتحدة. نقدم خدمات تأجير السيارات مع توصيل إلى باب منزلك وخدمة التسليم والاستلام من المطار، في جميع إمارات الدولة.</p>
</section>

<section id="about">
  <h2 id="about-title">من نحن</h2>
  <p id="about-text">راية الفخامة لتأجير السيارات هي شركة متميزة توفر لك تجربة سلسة وممتعة في استئجار السيارات مع خدمة عملاء متميزة وسهولة في التعامل.</p>
</section>

<section id="services">
  <h2 id="services-title">خدماتنا</h2>
  <div class="services">
    <div class="service-box">
      <h3 id="service1-title">تأجير يومي وشهري</h3>
      <p id="service1-text">اختر من مجموعة واسعة من السيارات لتلبية احتياجاتك اليومية أو الشهرية.</p>
    </div>
    <div class="service-box">
      <h3 id="service2-title">خدمة التوصيل</h3>
      <p id="service2-text">توصيل السيارة إلى باب منزلك أو استلامها من المطار في أي إمارة.</p>
    </div>
    <div class="service-box">
      <h3 id="service3-title">تأجير ينتهي بالتملك</h3>
      <p id="service3-text">استمتع بخيار تأجير السيارات مع إمكانية التملك لاحقاً.</p>
    </div>
  </div>
  
  <h2 id="gallery-title">معرض سياراتنا</h2>
  <div class="gallery">
    <img src="https://via.placeholder.com/400x200?text=Car+1" alt="Car 1">
    <img src="https://via.placeholder.com/400x200?text=Car+2" alt="Car 2">
    <img src="https://via.placeholder.com/400x200?text=Car+3" alt="Car 3">
    <img src="https://via.placeholder.com/400x200?text=Car+4" alt="Car 4">
  </div>
</section>

<section id="pricing">
  <h2 id="pricing-title">أسعار السيارات</h2>
  <div class="pricing">
    <div class="car-box">
      <img src="https://via.placeholder.com/400x150?text=Car+1" alt="Car 1">
      <h3>تويوتا كامري</h3>
      <p>السعر اليومي: 150 درهم | السعر الشهري: 3500 درهم</p>
      <button onclick="showBooking('تويوتا كامري')">احجز الآن</button>
    </div>
    <div class="car-box">
      <img src="https://via.placeholder.com/400x150?text=Car+2" alt="Car 2">
      <h3>نيسان سنترا</h3>
      <p>السعر اليومي: 120 درهم | السعر الشهري: 3000 درهم</p>
      <button onclick="showBooking('نيسان سنترا')">احجز الآن</button>
    </div>
    <div class="car-box">
      <img src="https://via.placeholder.com/400x150?text=Car+3" alt="Car 3">
      <h3>هوندا أكورد</h3>
      <p>السعر اليومي: 160 درهم | السعر الشهري: 3700 درهم</p>
      <button onclick="showBooking('هوندا أكورد')">احجز الآن</button>
    </div>
  </div>

  <div id="booking-form" style="display:none; margin-top:20px;">
    <h3 id="booking-title">نموذج الحجز</h3>
    <form id="form">
      <input type="text" id="name" placeholder="اسمك" required>
      <input type="email" id="email" placeholder="البريد الإلكتروني" required>
      <input type="tel" id="phone" placeholder="رقم الهاتف" required>
      <select id="car" required>
        <option value="">اختر السيارة</option>
        <option value="تويوتا كامري">تويوتا كامري</option>
        <option value="نيسان سنترا">نيسان سنترا</option>
        <option value="هوندا أكورد">هوندا أكورد</option>
      </select>
      <input type="date" id="startDate" required>
      <select id="duration" required>
        <option value="">مدة الإيجار</option>
        <option value="يومي">يومي</option>
        <option value="شهري">شهري</option>
      </select>
      <div style="display:flex; gap:10px;">
        <button type="button" onclick="sendEmail()">أرسل عبر البريد</button>
        <button type="button" onclick="sendWhatsApp()">أرسل عبر WhatsApp</button>
      </div>
    </form>
    <p id="confirmation" style="color:green; font-weight:bold; display:none;"></p>
  </div>
</section>

<section id="contact">
  <h2 id="contact-title">تواصل معنا</h2>
  <div class="contact">
    <div class="contact-box">
      <h3 id="contact-phone-title">الهاتف</h3>
      <p id="contact-phone">00971529290080</p>
    </div>
    <div class="contact-box">
      <h3 id="contact-email-title">البريد الإلكتروني</h3>
      <p id="contact-email">rayaalfhakhama@gmail.com</p>
    </div>
    <div class="contact-box">
      <h3 id="contact-map-title">الموقع</h3>
      <p><a id="contact-map" href="https://maps.app.goo.gl/5tUQ1Lg8wVdVstoo7" target="_blank">عرض على الخريطة</a></p>
    </div>
  </div>
</section>

<footer>
  &copy; 2025 <span id="footer-text">راية الفخامة لتأجير السيارات | Rayaalfakhama Rental Car</span>
</footer>

<div id="lightbox" onclick="this.style.display='none'">
  <img id="lightbox-img" src="">
</div>

<script>
// Switch language
const translations = {
  en: {
    title: "Rayaalfakhama Rental Car",
    navHome:"Home", navAbout:"About Us", navServices:"Services", navPricing:"Car Pricing", navContact:"Contact",
    homeTitle:"Welcome to Rayaalfakhama", homeText:"A leading car rental company in the UAE...",
    aboutTitle:"About Us", aboutText:"Rayaalfakhama Rental Car provides a smooth and enjoyable rental experience...",
    servicesTitle:"Our Services", service1Title:"Daily & Monthly Rentals", service1Text:"Choose from a wide range...",
    service2Title:"Delivery Service", service2Text:"Car delivery to your doorstep...", service3Title:"Rent-to-Own", service3Text:"Enjoy rent-to-own option...",
    galleryTitle:"Our Car Gallery",
    pricingTitle:"Car Pricing", bookingTitle:"Booking Form",
    contactTitle:"Contact Us", contactPhoneTitle:"Phone", contactPhone:"00971529290080",
    contactEmailTitle:"Email", contactEmail:"rayaalfhakhama@gmail.com",
    contactMapTitle:"Location", contactMap:"View on Map",
    footerText:"Rayaalfakhama Rental Car | راية الفخامة لتأجير السيارات"
  },
  ar: {
    title:"راية الفخامة لتأجير السيارات",
    navHome:"الرئيسية", navAbout:"من نحن", navServices:"خدماتنا", navPricing:"أسعار السيارات", navContact:"تواصل معنا",
    homeTitle:"مرحباً بكم في راية الفخامة", homeText:"شركة رائدة في تأجير السيارات...",
    aboutTitle:"من نحن", aboutText:"راية الفخامة لتأجير السيارات هي شركة متميزة...",
    servicesTitle:"خدماتنا", service1Title:"تأجير يومي وشهري", service1Text:"اختر من مجموعة واسعة...",
    service2Title:"خدمة التوصيل", service2Text:"توصيل السيارة إلى باب منزلك...", service3Title:"تأجير ينتهي بالتملك", service3Text:"استمتع بخيار تأجير السيارات...",
    galleryTitle:"معرض سياراتنا",
    pricingTitle:"أسعار السيارات", bookingTitle:"نموذج الحجز",
    contactTitle:"تواصل معنا", contactPhoneTitle:"الهاتف", contactPhone:"00971529290080",
    contactEmailTitle:"البريد الإلكتروني", contactEmail:"rayaalfhakhama@gmail.com",
    contactMapTitle:"الموقع", contactMap:"عرض على الخريطة",
    footerText:"راية الفخامة لتأجير السيارات | Rayaalfakhama Rental Car"
  }
};

function switchLanguage(lang){
  document.getElementById("title").innerText=translations[lang].title;
  document.getElementById("nav-home").innerText=translations[lang].navHome;
  document.getElementById("nav-about").innerText=translations[lang].navAbout;
  document.getElementById("nav-services").innerText=translations[lang].navServices;
  document.getElementById("nav-pricing").innerText=translations[lang].navPricing;
  document.getElementById("nav-contact").innerText=translations[lang].navContact;
  document.getElementById("home-title").innerText=translations[lang].homeTitle;
  document.getElementById("home-text").innerText=translations[lang].homeText;
  document.getElementById("about-title").innerText=translations[lang].aboutTitle;
  document.getElementById("about-text").innerText=translations[lang].aboutText;
  document.getElementById("services-title").innerText=translations[lang].servicesTitle;
  document.getElementById("service1-title").innerText=translations[lang].service1Title;
  document.getElementById("service1-text").innerText=translations[lang].service1Text;
  document.getElementById("service2-title").innerText=translations[lang].service2Title;
  document.getElementById("service2-text").innerText=translations[lang].service2Text;
  document.getElementById("service3-title").innerText=translations[lang].service3Title;
  document.getElementById("service3-text").innerText=translations[lang].service3Text;
  document.getElementById("gallery-title").innerText=translations[lang].galleryTitle;
  document.getElementById("pricing-title").innerText=translations[lang].pricingTitle;
  document.getElementById("booking-title").innerText=translations[lang].bookingTitle;
  document.getElementById("contact-title").innerText=translations[lang].contactTitle;
  document.getElementById("contact-phone-title").innerText=translations[lang].contactPhoneTitle;
  document.getElementById("contact-phone").innerText=translations[lang].contactPhone;
  document.getElementById("contact-email-title").innerText=translations[lang].contactEmailTitle;
  document.getElementById("contact-email").innerText=translations[lang].contactEmail;
  document.getElementById("contact-map-title").innerText=translations[lang].contactMapTitle;
  document.getElementById("contact-map").innerText=translations[lang].contactMap;
  document.getElementById("footer-text").innerText=translations[lang].footerText;
  document.body.dir=(lang==='ar')?'rtl':'ltr';
}

// Lightbox
document.querySelectorAll('.gallery img').forEach(img=>{
  img.addEventListener('click',()=>{document.getElementById('lightbox').style.display='flex';document.getElementById('lightbox-img').src=img.src;});
});

// Booking
function showBooking(carName){
  document.getElementById('booking-form').style.display='block';
  document.getElementById('car').value=carName;
}
function sendEmail() {
  const name=document.getElementById('name').value;
  const email=document.getElementById('email').value;
  const phone=document.getElementById('phone').value;
  const car=document.getElementById('car').value;
  const startDate=document.getElementById('startDate').value;
  const duration=document.getElementById('duration').value;
  const subject=`حجز سيارة - ${car}`;
  const body=`الاسم: ${name}%0D%0Aالبريد الإلكتروني: ${email}%0D%0Aالهاتف: ${phone}%0D%0Aالسيارة: ${car}%0D%0Aتاريخ البدء: ${startDate}%0D%0Aمدة الإيجار: ${duration}`;
  window.location.href=`mailto:rayaalfhakhama@gmail.com?subject=${subject}&body=${body}`;
  document.getElementById('confirmation').style.display='block';
  document.getElementById('confirmation').innerText='تم فتح البريد الإلكتروني لإرسال الحجز!';
}
function sendWhats
