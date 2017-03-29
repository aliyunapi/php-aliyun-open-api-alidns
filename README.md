# php-aliyun-open-api-alidns

Installation
------------

The preferred way to install this extension is through [composer](http://getcomposer.org/download/).

Either run

```
php composer.phar require --prefer-dist aliyunapi/php-aliyun-open-api-alidns
```

or add

```
"aliyunapi/php-aliyun-open-api-alidns": "~1.0"
```

to the require section of your composer.json.

使用方式
------------
```
$client = new \aliyun\alidns\Client([
    'accessKeyId' => '123456',
    'accessSecret' => '123456'
]);
$package = [
    'Action' => 'DescribeDomains',
];
$response = $client->createRequest($package);
print_r($response);
exit;
```