# Bismillahir rohmanir rohim

### `git` command line orqali ishlash bo'yicha o'rgangan qo'llanmalarimni saqlab borish uchun git commandalar ketma-ketligi

***
## `git bash` dasturi ichida yoziladigan commandlar

```html
mkdir git_lesson
```

`mkdir` - papka yaratish buyrug'i, `git_lesson` yangi papka nomi

```html
touch index.html
```

`touch` - yangi fayllarni yaratish uchun ishlatiladigan buyruq hisoblanadi.

### Agarda biror bir faylni `git bash` orqali o'chirmoqchi bo'lsak

```html
rm -rf index.html
```

ko'rinishida yozadigan bo'lsak mavjud bo'lgan `index.html` fayli o'chirib yuboriladi.

```html
git init
```

`git init` - biz turgan papkamizni `git` dan **nazorat**(ro'yxat)dan o'tkazish.

```html
git status
```

`git status` - ishlatilayotgan fayllni, papkalarni tekshirib turish uchun.

```html
git add
```

`git add` - mahalliy ombor(repository)ga qo'shish uchun tayyorlab beradi.
> `git add index.html` yoki `git add *.html` ko'rinishida yozilsa ma'lum bir faylni qo'shish uchun ishlatiladi agarda papkalarni qo'shmoqchi bo'lsak `git add /web` yoki `git add web` ko'rinishida yozsak ham papkani tayyorlab beradi.
> agarda bir barcha fayllarni ombor(repository)ga qo'shmoqchi bo'lsak `git addf .` ko'rinishi yozsak loyihamiz ichidagi barcha fayl va papkalarni ombor(repository)ga qo'shib beradi.

```html
git rm --cached file_name.type
```
bu yerda `git add` orqali qo'shilgan faylni paketdan chiqarib turish uchun ishlatiladi.

```html
git commit -m "Message"
```

`git commit -m "Message"` bu buyruq orqali biz `git add` qilib tayyorlab olgan fayllarimizni yuborishga tayyor qilib olamiz.

```html
git log
```

git orqali `git commit -m "Message"` qilib yuborilgan commitlarni yuborishdan oldin tekshirib olishimiz mumkin bo'ladi.

### Endi `git bash` dasturi orqali fayllarni yoki papkalarni code editorlarida ochishni ko'rib chiqamiz

1.`git bash` dasturining o'ziga biriktirilgan `vim` editoridan foydalanamiz, buning uchun bizga kerak bo'ladigan buyruq.
```html
vim index.html
```

ko'rinishida yozib olamiz va enter tugmasini bosamiz, ushbu tahrirlovchining imkoniyatlari juda ham kam shuning uchun kompyuterimizga `vscode` dasturini o'rnatib olishimiz kerak bo'ladi.

2.`Visual Studio Code` dasturi orqali fayllarni ochish usullari.
```html
code index.html
```

ushbu holatda yozadigan bo'lsak, biz aynan bir faylni `vscode` orqali ochib olishimiz mumkin bo'ladi.

3.`Visual Studio Code` orqali papkalarni ochish yo'llarini ko'ramiz.
```html
code papka_nomi
```

ko'rinishida yozadigan bo'lsak bizga tahrirlamoqchi bo'lgan papkamizni ochib beradi.

### `.gitignore` fayli haqida.

> Ushbu fayl `git status` orqali papka yoki fayllarni add qilishdan olib qolish uchun kerak bo'ladi, ushbu fayl ichida nima yozish kerak va sintaksis
> Agarda loyiham ichida index.html faylini commit qilmoqchi bo'lmasam ushbu ko'rinishda yozaman.
>> ```html
>> index.html
>> ```
> Agarda men barcha .html ko'rinishidagi fayllarni olmoqchi bo'lmasam ushbu ko'rinishda yozaman.
>> ```html
>> *.html
>> ```
> Agarda bir vaqtni o'zida bir nechta turdagi fayllarni ko'rinishini istamasam
> `.gitignore` faylini ichida
>> ```html
>> *.html
>> *.css
>> *.
>> ```

ko'rinishida yozishim mumkin va `.gitignore` faylini saqlayman va barchasi tayyor holatga o'tadi.

***

