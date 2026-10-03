# قدم بعدی: پس‌زمینهٔ طبیعی پاییزی (روی کامپیوتر خودت)

نسخهٔ فعلی (`index.html`) کار می‌کنه و همهٔ بررسی‌ها رو رد کرده. پس‌زمینه‌اش
گرافیکیه (برگ‌های طراحی‌شده و نور گرم). قدم بعدی اینه که جاش یه ویدیوی واقعی
و متحرک پاییزی بذاریم.

## متن دستور برای Claude Code

این پوشه (`videos/autumn-peelshot`) رو تو Claude Code باز کن و این رو بچسبون:

```
/hyperframes:hyperframes این یک پروژهٔ موجود HyperFrames است (BRIEF.md و NEXT-STEPS.md را بخوان).
ویرایش مشخص: پس‌زمینهٔ گرافیکی پاییزی را با یک ویدیوی طبیعی و متحرک پاییزی عوض کن.
۱) با Higgsfield (مدل seedance_2_5، نسبت 1:1، ۵ ثانیه، 1080p، بدون صدا) ویدیو را
   با «پرامپت ویدیوی پس‌زمینه» در NEXT-STEPS.md بساز و در assets/autumn-bg.mp4 ذخیره کن.
   اگر Higgsfield در دسترس نبود، بگو تا خودم از سایتش دانلود کنم.
۲) در index.html ویدیو را به‌صورت <video> بی‌صدا در پایین‌ترین لایه (زیر همه‌چیز) بگذار
   و #sun، #bokeh، #ground، #pile-back و #leaves-back را حذف کن. محصول،
   برگ‌های جلوی محصول، شعار فارسی، نور (light leak) و گرین را نگه دار.
۳) npm run check و اسنپ‌شات‌ها را اجرا کن، یک فریم نشانم بده و بعد از تأیید من رندر بگیر.
```

## پرامپت ویدیوی پس‌زمینه (برای Higgsfield)

> Photorealistic autumn forest at golden hour, static locked-off camera with a very slow gentle
> push-in. Warm sunlight streams through orange and red maple trees, soft god rays, shallow depth
> of field with creamy bokeh. Golden and red leaves drift slowly down through the air and a light
> breeze moves the branches. The lower third of the frame is a soft out-of-focus forest floor
> covered with fallen autumn leaves, and the center is open empty space for a product to be placed
> later. No people, no animals, no text, no objects.

تنظیمات: مدل `seedance_2_5`، `aspect_ratio: 1:1`، `duration: 5`، `resolution: 1080p`،
`generate_audio: false`. هزینهٔ تقریبی: **۶۰ کردیت**.

## بدون Higgsfield

می‌تونی هر ویدیوی طبیعی پاییزی (حداقل ۵ ثانیه، ترجیحاً مربعی) رو با اسم
`assets/autumn-bg.mp4` ذخیره کنی و فقط قدم‌های ۲ و ۳ دستور بالا رو بزنی.
