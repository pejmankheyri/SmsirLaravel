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

# Send SMS by Laravel

A practical package for sending SMS through the sms.ir panel

## Installation

</div>

<div>

```
composer require pejmankheyri/smsirlaravel
php artisan vendor:publish
php artisan migrate
```

</div>

<div dir="rtl">

## Features

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

## Settings

* Add this code in the `app.php` file in the providers section: `pejmankheyri\smsirlaravel\SmsirlaravelServiceProvider::class,`
* Add this code in the `app.php` file in the aliases section: `'Smsirlaravel' => pejmankheyri\smsirlaravel\SmsirlaravelFacade::class,`
* After publishing the package, open the `smsirlaravel.php` file in the config folder and make the settings as below:

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

## Development Assistance

We welcome pull requests.

For major changes, please open an issue first so we can discuss what you want to change.

## License

MIT

</div>
