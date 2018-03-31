3/30 - start reading

	pid1. 'Neural Machine Translation in Linear Time', Kalchbrenner et al. 2017
		=> 
	pid2. 'Recurrent Continuous Translation Models', Kalchbrenner et al. 2013
		=> tried this one upon knowing that this paper suggests basic building block
			used at pid1. 
		=> Suggests CNN encoder - ___REST TO KNOW____

Requirements
============

* PHP >= 5.3.7
* cURL Extension

Installation
============

    composer require buonzz/laravel-4-freegeoip:dev-master

Add the service provider and facade in your config/app.php

Service Provider

    Buonzz\GeoIP\Laravel4\ServiceProviders\GeoIPServiceProvider

Facade

    'GeoIP'            => 'Buonzz\GeoIP\Laravel4\Facades\GeoIP',


Usage
=====

Get country of the visitor

    GeoIP::getCountry();  // returns "United States"
    
Get country code of the visitor

    GeoIP::getCountryCode();  // returns "US"

Get region of the visitor


Credits
=======

* Alexandre Fiori for the awesome http://freegeoip.net web api
* MaxMind for the data
