# Sozlash (Setup)

## Muhit (Environment)

Boshlashdan oldin [Ruby](https://www.ruby-lang.org/en/documentation/installation/) va [NodeJS](https://nodejs.org/) tizimingizda o‘rnatilganligiga ishonch hosil qiling.

Keyin Jekyll'ni o‘rnating:

```
$ gem install jekyll
```

So‘ng Gulp mijozini o‘rnating:

```
$ npm install gulp-cli -g
```

---

## Shablonni o‘rnatish (Installing template)

1. [Jekflix Template](https://github.com/thiagorossener/jekflix-template/fork) loyihasini **fork** qiling (nusxa oling)
2. Endi siz fork qilgan repozitoriyadan nusxa oling:

```
$ git clone https://github.com/<sizning-github-usernameingiz>/jekflix-template.git
```

3. Loyihaning lokal papkasiga o‘ting:

```
$ cd path/to/jekyll-template
```

4. npm paketlarini o‘rnating:

```
$ npm install
```

5. Ruby kutubxonalarini o‘rnating:

```
$ bundle install
```

6. Jekyll loyihasini build qiling (tayyorlash):

```
$ bundle exec jekyll build
```

7. So‘ngra Gulp'ni ishga tushuring:

```
$ gulp
```

---

## Mahalliy ishga tushirish (Running local)

Yuqoridagi bosqichlardan so‘ng, Jekyll'ni lokalda ishga tushirish uchun faqat quyidagini bajaring:

```
$ gulp
```

---

## Moslashtirish (Customization)

*Jekflix Template* sizga ko‘plab sozlamalar orqali saytni shaxsiylashtirish imkonini beradi. Batafsil ma’lumot uchun [sozlamalar hujjatini](settings.md#settings) ko‘rib chiqing.

Murakkab dizayn (tema) sozlash uchun `_sass` papkasidagi uslub fayllariga murojaat qiling.

---

## Tarjimalar (Translations)

Mavzu bo‘ylab matnlarni tarjima qilish uchun `src/yml` papkasi ichida `translations.yml` nomli fayl yarating va quyidagi sozlamalarni kiriting:

> **Eslatma:** Agar siz shablonni `gem` sifatida ishlatayotgan bo‘lsangiz, bu ma’lumotlarni faqat `_config.yml` fayliga qo‘shing.

```yaml
translations:
  text:
    new_post: "Yangi post"
    see_also: "Shuningdek qarang"
    search: "Qidirish"
    author: "Muallif"
    share: "Ulashish"
    comments: "Izohlar"
  button:
    read_now: "Hozir o‘qish"
    share_on_twitter: "Twitter’da ulashish"
    share_on_facebook: "Facebook’da ulashish"
  pagination:
    page: "Sahifa"
    of: "dan"
    next_page: "Keyingi sahifa"
    next_post: "Oldingi sahifa"
  recommendation:
    text: "Nega keyingisini o‘qib ko‘rmaysiz?"
    back_btn: "Yuqoriga qaytish"
  error_404:
    title: "Sahifa topilmadi :("
    message: "Kechirasiz. Qidirgan sahifangiz topilmadi."
    image_alt: "404 - Sahifa topilmadi"
  contact:
    title: "Men bilan bog‘laning"
    subject: "Yangi murojaat!"
    submit_btn: "Yuborish"
    placeholders:
      name: "Ismingiz"
      email: "Elektron pochtangiz"
      message: "Xabaringiz"
    errors:
      locale: "uz"
      empty_name: "Ism majburiy"
      empty_email: "Email majburiy"
      invalid_email: "Email noto‘g‘ri"
      empty_message: "Xabar majburiy"
    after_send:
      title: "Xabar yuborildi!"
      message: "Xabaringiz uchun rahmat. Tez orada javob beraman."
```

---
