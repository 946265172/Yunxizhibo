### ��Ϭֱ��PHP-SDK, �ٷ�API����
@author  holger <whjsjq@gmail.com>
@link
@version 1.0

### �ֶ�����
```php
require_once('/path/to/Yunxizhibo-php/Yunxizhibo.php');
```

### ���뷽��
### ��ʼ��
```php
$accessKey = 'accessKey';
$secretKey = 'secretKey';
 ```

### ��дAccessKey��SecretKey
 ```php
$yxObj = new Yunxizhibo($accessKey, $secretKey);
 ```

###��ȡ��б�
```php
$data = $yxObj->getActivityList();

if(empty($data)) {
   echo $yxObj->$errCode;
   echo $yxObj->$errMsg;
}
```
### �б�
 ```php
$list = $data["activitys"];
```
### ҳ��
 ```php
$pageCount = $data["pageCount"];
```

### ��ȡ�����
 ```php
 $data = $yxObj->getActivityInfo();

if(empty($data)) {
   echo $yxObj->$errCode;
   echo $yxObj->$errMsg;
}
```

### �����
```php
$activity = $data["activity"];
```


### ��ȡֱ����Ƶ����
```php
$data = $yxObj->getLivestreamInfo();

if(empty($data)) {
   echo $yxObj->$errCode;
   echo $yxObj->$errMsg;
}
```
### ֱ����Ƶ����
```php
$livestream = $data["livestream"];
```
### ΢��Ƕ���ַ
```php
$wechatPlayUrl = $data["wechatPlayUrl"];
```
### ��ҳǶ���ַ
```php
$webPlayUrl = $data["webPlayUrl"];
```
### appǶ���ַ
```php
$appPlayUrl = $data["appPlayUrl"];
```
### ������Ƕ���ַ
```php
$embedPlayerUrl = $data["embedPlayerUrl"];
```
### Χ������
```php
$totalNum = $data["totalNum"];
```

