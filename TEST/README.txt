FreeGeoIP for Laravel 4 
=======================

[![Build Status](https://travis-ci.org/buonzz/laravel-4-freegeoip.svg?branch=master)](https://travis-ci.org/buonzz/laravel-4-freegeoip)
[![Latest Stable Version](https://poser.pugx.org/buonzz/laravel-4-freegeoip/v/stable.svg)](https://packagist.org/packages/buonzz/laravel-4-freegeoip) [![Total Downloads](https://poser.pugx.org/buonzz/laravel-4-freegeoip/downloads.svg)](https://packagist.org/packages/buonzz/laravel-4-freegeoip)
[![Latest Unstable Version](https://poser.pugx.org/buonzz/laravel-4-freegeoip/v/unstable.svg)](https://packagist.org/packages/buonzz/laravel-4-freegeoip) [![License](https://poser.pugx.org/buonzz/laravel-4-freegeoip/license.svg)](https://packagist.org/packages/buonzz/laravel-4-freegeoip)

Laravel 4 Library for calling http://freegeoip.net/ API.

In contrary to all other packages wherein it requires that you have the geoip database in your filesystem, this library calls a free service
So you dont really have to worry about downloading and maintaining geoip data from Maxmind in your own server.

Just install the package, add the config and it is ready to use!


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