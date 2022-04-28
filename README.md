
   #زبان راهنما : فارسی
   زبان های راهنما : فارسی
	

	
   ## مراحل خیلی ابتدایی
   1. اگر پایتون در سیستم شما نصب نیست ، پایتون را از [اینجا](https://www.python.org/downloads/windows/) دانلود کنید و سپس نصب کنید.
   2. برنامه git را از طریق این [لینک](https://git-scm.com/download/win) دانلود و سپس نصب کنید.
   3. از طریق این [لینک](https://signup.heroku.com/login) در وبسایت Heroku ثبت نام کنید.
   4. برنامه Heroku CLI را از طریق این [لینک](https://devcenter.heroku.com/articles/heroku-cli) دانلود و نصب کنید.
	
   ### مرحله 0 :

   - برای شروع با استفاده از دستور زیر این repository را clone کنید و سپس طبق مراحل زیر تغییرات مختص به خودتان را انجام بدهید. 
<div dir="ltr">
  
   -  ```shell
      git clone https://github.com/Sajad-m/Project-Heroku.git
   -  ```shell
      cd Project-Heroku   
</div>

   ### مرحله یک :

   - بر روی bot.py کلیک راست کنید و کد های مربوط بات خودتان را در آن جایگزاری کنید و سپس فایل را ذخیره کنیدو ببنید.

   
   ### مرحله دوم :

   - اگر شما میخواهید نام فایل *bot.py* را تغییر دهید ، باید بعد از تغییر ، محتوای فایل *Procfile* را نیز تغییر دهید ، یعنی آنکه بر روی *Procfile* کلیک راست کنید
	و سپس Edit with notepad را بزنید و به شکل کد زیر محتوا را تغییر بدهید یعنی بجای *Project.py* نام فایلی که کدتان درآن قرار دارد را بزنید.
 <div dir="ltr">

   -  ```shell
      worker: python Project.py
</div>
   
   ### مرحله سوم :

- نام هر ماژول یا کتاب خانه ای که داخل پروژه و سورس کد خود استفاده کرده اید را در فایل *requirements.txt* وارد کنید. 

	- به طور مثال چندین ماژول را در *requirements.txt* وارد کرده ایم :
<div dir="ltr">
	    
	mutagen
	gtts
	rubika
</div>

### مرحله چهارم :
- محیط Bash یا CMD را باز کنید و به محلی که فایل هایتان یعنی *bot.py* قرار دارد ، بروید. 
- در همان محیط با کمک کد زیر ، git را راه اندازی کنید.

<div dir="ltr">
  
   -  ```shell
      git init	   
</div>

### مرحله پنجم :
- heroku CLI را نصب کنید.
- سپس دستور زیر را وارد کنید : 

<div dir="ltr">
  
   -  ```shell
      heroku login
      heroku create app_name	   
</div>

- اگر از قبل یک اپلیکیشن در وبسایت Heroku ساخته اید ، از کد زیر استفاده کنید و نام اپلیکیشن خود را جاگزین app_name کنید.

 <div dir="ltr">
  
   -  ```shell
      heroku git:remote -a app_name	   
</div>

 - در ادامه کد زیر را وارد کنید ، دقت کنید که با استفاده از این کد ، در حقیقت پروژه خود را بر Heroku آپلود کرده اید :
 <div dir="ltr">
  
   -  ```shell
      git add -f bot.py Procfile rules.txt help.txt requirements.txt __init__.py
   -  ```shell
      git commit -m "Added Files"	   
</div>
     
  
- با استفاده از دستور زیر ، آپلود فایل هایتان آغاز میشود و بر وبسایت Heroku قرار میگیرد.
 <div dir="ltr">
  
   -  ```shell
      git push heroku master   
</div>
- اگر در هنگام وارد کردن کد بالا با ارور مواجه شدید ، کد زیر را وارد نمایید :

<div dir="ltr">
  
   -  ```shell
      git push heroku master  --force 
</div>

### تبریک ، ربات شما در تلگرام ران شد ، اگر ران نبود با استفاده از کد زیر اطمینان حاصل کنید : 
 
 <div dir="ltr">
  
   -  ```shell
      heroku ps
</div>


- اگر ران نشده بود با استفاده از کد زیر dynos را ریست میکنیم :
  
 <div dir="ltr">
  
   -  ```shell
      heroku ps:scale worker=0
   -  ```shell
      heroku ps:scale worker=1
</div>


- حالا باید ران شده باشد ، امیدواریم از این آموزش لذت برده باشید. 
   
### تماس با ما :	
<div dir="ltr">
  
  -  ```shell
      Telegram : @Sajad_Venus
      Rubika : @Sajad_Venus   
</div>

   
   
   
   
   
   
   
   
   
   
   
   
   
   
   
   

