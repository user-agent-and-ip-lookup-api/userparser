# User Agent Parser and IP Address Lookup API
**Userparser** is a user-agent parser & IP-address lookup API that transforms user agent strings into rich metadata and usage analytics. Sign up and start receiving parsed user-agent & ip-address data instantly to detect country, browser, OS, device, and crawler in real-time with our secure user-agent string & IP-address Lookup API..

This free user-agent parser and IP-address lookup tool enables developers to determine what type of device a user is using and where he is making the request. To assist them in creating more engaging user experiences.

With this tool, you can easily parse user agents and extract information such as device type, device name, device brand, device viewport width, device viewport height, operating system name, operating system version, browser name, browser version, crawler name, crawler category, crawler owner, crawler URL, and so on.

You can easily perform an IP-address lookup with this tool and extract information such as country name, country code, calling code, currency code, capital city, continent name and continent code, and so on.

# Features & Integration
* **Country name** It can assist you in determining the visitor country so that you can display your content based on the user's location.
* **Device viewport:** It will provide you the user's device viewport (height and width), so you can customize your UX interface. 
* **Device name:** Unlike other providers This User Agent parser API has incredible good in returning user device name (especially if the user is using Smartphone), It informs you his/her device name is Infinix Note 10 instead of only Note 10 (helps you prevent confusions from a lot of other brands Note 10).
* **Device type:** It will inform you the device type which is weight it is Mobile, Tablet, Computer, or Crawler effectively. So you can customize you web design better.
* **Crawler Detection:** is accurate for most of the crawlers out there. You can get Crawler name, crawler Owner, crawler category (Search-engine, Scrapers, Monitors, Marketing etc...) Crawler URL and crawler last seen. So you can differ your crawlers as well as your real users.
* **Full Lookup:** Parsing User Agent and IP address lookup in all Plans is the same; it returns the same information regardless of plan, with the exception of API call limits per day and month.
** All in one API call** You can get all the data with a single API call. You can send your user's IP address or/and user-agent for lookup and then get your data all in one request.
* **JSON & XML API:** The userparser API is capable of delivering API results in JSON or XML format.
* **Free for Ever:** It allows you to use it for free for up to 10,000 API calls per month for free for ever, so you can decide to upgrade or remain in the Free plan. You have an option to upgrade, downgrade and even cancel your subscription at any time, And it have a custom plans if you want too.
* **Customer support:** Even in the free plan, it has excellent email support from its developers, and the higher plans have preferred and dedicated support.
# Documentation
An in-depth API documentation, including interactive code examples and extensive descriptions can be found at (https://www.userparser.com/docs/user-agent-and-geoip-lookup-api-v1.1)
## PHP code Example
```php
$json_url = "https://api.userparser.com/1.1/detect?ua=YOUR_USER_AGENT&ip=$ip_address&api_key=YOUR_API_KEY";
$ch = curl_init();
curl_setopt($ch, CURLOPT_SSL_VERIFYPEER, false);
curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
curl_setopt($ch, CURLOPT_TIMEOUT, 1);
curl_setopt($ch, CURLOPT_URL, $json_url);
$result = curl_exec($ch);
curl_close($ch);
$json_data = json_decode($result);
if($json_data->info->status == "success"){
    $real_country = $json_data->location->countryName;
    $countryCode2 = $json_data->location->countryCode2;
    $countryCode3 = $json_data->location->countryCode3;
    $capitalCity = $json_data->location->capitalCity;
    $continentName = $json_data->location->continentName;
    $continentCode = $json_data->location->continentCode;
    $callingCode = $json_data->location->callingCode;
    $currencyCode = $json_data->location->currencyCode;
    $browserName =$json_data->browser->name;
    $browserVersion = $json_data->browser->version;
    $browserFullVersion = $json_data->browser->fullVersion;
    $renderEngine = $json_data->browser->engine;
    $osName = $json_data->operatingSystem->name;
    $osVersion = $json_data->operatingSystem->version;
    $deviceName = $json_data->device->name;
    $deviceType = $json_data->device->type;
    $isTouchScreen = $json_data->device->isTouchScreen;
    $device_brand = $json_data->device->brand;
    $device_width = $json_data->device->screenResolutionWidth;
    $device_height = $json_data->device->screenResolutionHeight;
    $viewport_screen_width = $json_data->device->viewportWidth;
    $viewport_screen_height = $json_data->device->viewportHeight;
    $languageDetection = $json_data->device->language;
    $is_mobile = $json_data->device->isMobile;
    $userAgent = $json_data->info->ua;
    $isCrawler = $json_data->crawler->isCrawler;
    $crawlerName = $json_data->crawler->name;
    $crawlerOwner = $json_data->crawler->owner;
    $crawlerCategory = $json_data->crawler->category;
    $crawlerUrl = $json_data->crawler->url;
    $crawlerLastSeen = $json_data->crawler->lastSeen;
}
```
# JSON response 
```JSON
  {
    "info": {
        "status": "success",
        "message": "The user agent was parsed and ip lookup was completed successfully.",
        "ua": "Mozilla/5.0 (Linux; Android 11; SM-A505F) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/98.0.4758.101 Mobile Safari/537.36"
    },
    "browser": {
        "name": "Chrome",
        "version": "98",
        "fullVersion": "98.0.4758.101",
        "engine": "Blink"
    },
    "operatingSystem": {
        "name": "Android",
        "version": "11"
    },
    "device": {
        "name": "Samsung Galaxy A50",
        "type": "Smartphone",
        "brand": "Samsung",
        "screenResolutionWidth": "1080px",
        "screenResolutionHeight": "2340px",
        "viewportWidth": "412px",
        "viewportHeight": "756px",
        "language": null,
        "isTouchScreen": true,
        "isMobile": true
    },
    "crawler": {
        "isCrawler": false,
        "name": null,
        "owner": null,
        "category": null,
        "url": null,
        "lastSeen": null
    },
        "location": {
        "countryName": "Italy",
        "countryCode2": "IT",
        "countryCode3": "ITA",
        "capitalCity": "Rome",
        "continentName": "Europe",
        "continentCode": "EU",
        "callingCode": "+39",
        "currencyCode": "EUR"
    }
}
  
```
Continue reading an in-depth API documentation [here](https://www.userparser.com/docs/user-agent-and-geoip-lookup-api-v1.1).
# Customer Support

Need any assistance? Get in touch with Customer Support
[Customer Support](https://www.userparser.com/contact-us).

# Legal

All usage of the userparser website, API, and services is subject to the userparser [Terms & Conditions](https://www.userparser.com/terms-of-use).

