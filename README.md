<p align="center">
<img src="https://user-images.githubusercontent.com/3329008/111814382-a31bc700-88ef-11eb-94e2-41dd10c0d2b1.png" /> + 
<img src="https://user-images.githubusercontent.com/3329008/114069542-586ce980-98b4-11eb-8e18-c625cb8812d1.png" />
</p>
<p align="center">
  <a href="https://packagist.org/packages/pejmankheyri/smsirlaravel"><img src="https://poser.pugx.org/pejmankheyri/smsirlaravel/v/stable" alt="version"></a>
<a href="https://packagist.org/packages/pejmankheyri/smsirlaravel"><img src="https://img.shields.io/packagist/dt/pejmankheyri/smsirlaravel" alt="Total Downloads"></a>
  <a href="https://packagist.org/packages/pejmankheyri/smsirlaravel"><img src="https://poser.pugx.org/pejmankheyri/smsirlaravel/d/monthly" alt="Monthly Downloads"></a>
<a href="https://packagist.org/packages/pejmankheyri/smsirlaravel"><img src="https://img.shields.io/github/license/pejmankheyri/smsirlaravel" alt="License"></a>
</p>
<div dir="rtl">

# ارسال پیامک توسط لاراول

یک پکیج کاربردی برای ارسال پیامک از طریق پنل sms.ir

## نصب

</div>

<div>

```
composer require pejmankheyri/smsirlaravel
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

* این کد را در فایل `app.php` بخش providers اضافه کنید: `pejmankheyri\smsirlaravel\SmsirlaravelServiceProvider::class,`
* این کد را در فایل `app.php` بخش aliases اضافه کنید: `'Smsirlaravel' => pejmankheyri\smsirlaravel\SmsirlaravelFacade::class,`
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