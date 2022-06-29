# User Agent Parser
**UserParser** is a user Agent parser API that transforms user agent strings into rich metadata and usage analytics.
To Detect any Browser, OS, Device and Crawler in Real-Time with our Secure User-Agent String Lookup API you have to Sign up and start getting Parsed User Agent data instantly.

This Free User Agent Parser allows developers to detect what type of device a user is using. To help them to create more engaging experiences for users.

With this tool, you can easily parse user agents and extract information about the device type, device name, device brand, device viewport width, device viewport height, operating system name, operating system version browser name, browser version, crawler name, crawler category, crawler owner, crawler URL, etc...


# Features & Integration
* **Device viewport:** It will provide you the user's device viewport (height and width), so you can customize your UX interface. 
* **Device name:** Unlike other providers This User Agent Parser API has incredible good in returning user device name (especially if the user is using Smartphone), It informs you his/her device name is Infinix Note 10 instead of only Note 10 (helps you prevent confusions from a lot of other brands Note 10).
* **Device type:** It will inform you the device type which is weight it is Mobile, Tablet, Computer, or Crawler effectively. So you can customize you web design better.
* **Crawler Detection:** is accurate for most of the crawlers out there. You can get Crawler name, crawler Owner, crawler category (Search-engine, Scrapers, Monitors, Marketing etc...) Crawler URL and crawler last seen. So you can differ your crawlers as well as your real users.
* **Full parsing:** Parsing User Agent in all Plans is equal it gives same info regardless of plans except limitations per month.
* **JSON & XML API:** The userparser API is capable of delivering API results in JSON or XML format.
* **Free for Ever:** It allows you to use it for free for up to 10,000 API calls per month for free for ever, so you can decide to upgrade or remain in the Free plan. You have an option to upgrade, downgrade and even cancel your subscription at any time, And it have a custom plans if you want too.
* **Customer support:** It have a great fast reply Email support from its developers even in the Free plan and have Preferred and Dedicated support in the higher plan.
# Documentation
An in-depth API documentation, including interactive code examples and extensive descriptions can be found at https://www.userparser.com/docs/user-agent-parser-api-documentation-v1.0.0
## PHP code Example
```php
$json_url = "https://api.userparser.com/api/1.0.0/detect?ua=YOUR_USER_AGENT&api_key=YOUR_API_KEY";
$ch = curl_init();
curl_setopt($ch, CURLOPT_SSL_VERIFYPEER, false);
curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
curl_setopt($ch, CURLOPT_URL, $json_url);
$result = curl_exec($ch);
curl_close($ch);
$json_data = json_decode($result);
if($json_data->info->status == "success"){
    $brawserName = $json_data->browser->name;
    $browserVersion = $json_data->browser->version;
    $browserFullVersion = $json_data->browser->fullVersion;
    $renderEngine = $json_data->browser->engine;
    $osName = $json_data->operatingSystem->name;
    $osVersion = $json_data->operatingSystem->version;
    $deviceName = $json_data->device->name;
    $deviceType = $json_data->device->type;
    $deviceBrand = $json_data->device->brand;
    $screenWidth = $json_data->device->screenResolutionWidth;
    $screenHeight = $json_data->device->screenResolutionHeight;
    $viewportScreenWidth = $json_data->device->viewportScreenWidth;
    $viewportScreenHeight = $json_data->device->viewportScreenHeight;
    $languageDetection = $json_data->device->language;
    $isTouchScreen = $json_data->device->isTouchScreen;
    $isMobile = $json_data->device->isMobile;
    $apiResultMessage = $json_data->info->message;
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
        "message": "The user agent was parsed successfully.",
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
    }
}
```
Continue reading an in-depth API documentation [here](https://www.userparser.com/docs/user-agent-parser-api-documentation-v1.0.0).
# Customer Support

Need any assistance? Get in touch with Customer Support
[Customer Support](https://www.userparser.com/contact-us).

# Legal

All usage of the userparser website, API, and services is subject to the userparser [Terms & Conditions](https://www.userparser.com/terms-of-use).

