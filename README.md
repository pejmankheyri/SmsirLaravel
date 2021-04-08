<p align="center">
<img src="https://user-images.githubusercontent.com/3329008/111814382-a31bc700-88ef-11eb-94e2-41dd10c0d2b1.png" /> + 
<img src="https://user-images.githubusercontent.com/3329008/114069542-586ce980-98b4-11eb-8e18-c625cb8812d1.png" />
</p>
<p align="center">
  <a href="https://packagist.org/packages/pejmankheyri/smsir-smsirlaravel"><img src="https://poser.pugx.org/pejmankheyri/smsir-smsirlaravel/v/stable" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/pejmankheyri/smsir-smsirlaravel"><img src="https://img.shields.io/packagist/dt/pejmankheyri/smsir-smsirlaravel" alt="Total Downloads"></a>
  <a href="https://packagist.org/packages/pejmankheyri/smsir-smsirlaravel"><img src="https://poser.pugx.org/pejmankheyri/smsir-smsirlaravel/d/monthly" alt="Monthly Downloads"></a>

</p>
<div dir="rtl">

# ارسال پیامک توسط لاراول

یک پکیج کاربردی برای ارسال پیامک از طریق پنل sms.ir


> [نصب](https://github.com/pejmankheyri/SMSIR-SmsirLaravel#%D9%86%D8%B5%D8%A8)
> 
> [امکانات](https://github.com/pejmankheyri/SMSIR-SmsirLaravel#%D8%A7%D9%85%DA%A9%D8%A7%D9%86%D8%A7%D8%AA)
> 
> [تنظیمات](https://github.com/pejmankheyri/SMSIR-SmsirLaravel#%D8%AA%D9%86%D8%B8%DB%8C%D9%85%D8%A7%D8%AA)
> 
> [کمک به توسعه](https://github.com/pejmankheyri/SMSIR-SmsirLaravel#%DA%A9%D9%85%DA%A9-%D8%A8%D9%87-%D8%AA%D9%88%D8%B3%D8%B9%D9%87)
> 
> [لایسنس](https://github.com/pejmankheyri/SMSIR-SmsirLaravel#%D9%84%D8%A7%DB%8C%D8%B3%D9%86%D8%B3)

## نصب با آپلود فایل

</div>

<div>

```
composer require ipecompany/smsirlaravel
php artisan vendor:publish
php artisan migrate
```

</div>

<div dir="rtl">

## امکانات

</div>

* `Smsirlaravel::send()`
* `Smsirlaravel::credit()`
* `Smsirlaravel::getLines()`
* `Smsirlaravel::addToCustomerClub()`
* `Smsirlaravel::deleteContact()`
* `Smsirlaravel::sendToCustomerClub()`
* `Smsirlaravel::addContactAndSend()`
* `Smsirlaravel::sendVerification()`
* `Smsirlaravel::ultraFastSend()`
* `Smsirlaravel::getSentMessages()`
* `Smsirlaravel::getReceivedMessages()`

<div dir="rtl">

## تنظیمات

* این کد را در فایل `app.php` بخش providers اضافه کنید: `ipecompany\smsirlaravel\SmsirlaravelServiceProvider::class,`
* این کد را در فایل `app.php` بخش aliases اضافه کنید: `'Smsirlaravel' => ipecompany\smsirlaravel\SmsirlaravelFacade::class,`
* بعد از publish کردن پکیج فایل `smsirlaravel.php` را در پوشه config باز کنید و تنظیمات را مانند زیر انجام دهید:

</div>

<div>

```
'webservice-url' => env('SMSIR-WEBSERVICE-URL','https://ws.sms.ir/'),
'api-key' => env('SMSIR-API-KEY','Your sms.ir api key'),
'secret-key' => env('SMSIR-SECRET-KEY','Your sms.ir secret key'),
'line-number' => env('SMSIR-LINE-NUMBER','Your sms.ir line number'
```

</div>

<div dir="rtl">

## کمک به توسعه

از Pull request ها استقبال می کنیم.

برای تغییرات عمده ، لطفاً ابتدا یک issue را باز کنید تا در مورد آنچه می خواهید تغییر دهیم و بحث کنیم.

## لایسنس

MIT

</div>