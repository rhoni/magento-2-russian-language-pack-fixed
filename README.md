# Magento 2 Russian Language Pack (Fixed)

**Magento 2 Russian Language Pack** enables you to customize the existing language and adjust to Russian Language, that is really perfect tool to localize your store in Russia. This package will allow you to convert all words and phrases from both the frontend and the backend into the Russian Language.

Today, in Magento 2 Russian Language Pack topic, I will instruct you to download and install the package. After all, the automatic translation is implemented right after you activate Russian (Russia) option in `Store > Configuration > Locale Options`.

## 1. How to Install Russian Language Pack

There are 3 different methods to install this language pack.

### ✓ Method #1. Composer method (Recommend)

Install the Russian language pack via composer is never easier.

**Install Russian pack**:

```
composer require rhoni/magento-2-russian-language-pack-fixed:dev-master
php bin/magento setup:static-content:deploy ru_RU
php bin/magento indexer:reindex
php bin/magento cache:clean
php bin/magento cache:flush

```


**Update  Russian pack**:

```
composer update rhoni/magento-2-russian-language-pack-fixed:dev-master
php bin/magento setup:static-content:deploy ru_RU
php bin/magento indexer:reindex
php bin/magento cache:clean
php bin/magento cache:flush

```

### ✓ Method #2. Copy & Paste method (Not recommended)

This method suitable for non-technical people such as merchants. Just download the package then flush cache.

**Overview**

- Step 1: Download the Russian language pack
- Step 2: Unzip Russian pack
- Step 3: Flush Magento 2 Cache

#### Step 1 : Download the Russian language pack

You can download the language pack

#### Step 2: Unzip Russian pack

Unzip the Russian language pack to Magento 2 root folder. In this guide, we extract to `/var/www/html/`
Your Magento 2 root folder can be: `/home/account_name/yourstore.com/public_html/`

```
unzip master.zip app/i18n/Rhoni/

```

Rename folder `magento-2-russian-language-pack-fixed` to `ru_ru`.


You also can unzip locally and upload them to Magento 2 root folder.

#### Step 3: Flush Magento 2 Cache

```
php bin/magento cache:clean
php bin/magento cache:flush

```

### ✓ Method #3. Download and install manually (Not recommended)

To download and install Russian pack manually, you have to access to your server via FTP or SFTP.

#### Step 1: Download the package

- [Download .zip](https://github.com/rhoni/magento-2-russian-language-pack-fixed/archive/master.zip)
- [Download .tar.gz](https://github.com/rhoni/magento-2-russian-language-pack-fixed/tarball/master)

#### Step 1: Unzip and upload

Unzip the compressed file and upload file `master.zip` into `app/i18n/Rhoni/ru_ru/`

This language pack code is: **ru_ru**

#### Step 2: Flush cache

```
php bin/magento cache:clean
php bin/magento cache:flush

```

## 3. How to Active the Russian language pack 

Now time to active the Russian language pack for your Magento 2 store. From Magento 2 admin panel, navigate to `Stores > Configuration > General > Locale Options`
![{{Magento 2 Russian language pack}}](https://camo.githubusercontent.com/5e1749085c3a4ba69b1184e84c5705c7dff33ff1/68747470733a2f2f63646e2e6d616765706c617a612e636f6d2f6d656469612f67656e6572616c2f6150535541306c2e706e67)


## 4. How to contribute

Contribute to this language at :
- On Github - It's faster, our team will approve it after you send pull request.

## 5. Supported Magento versions

It supports all Magento 2 versions include Magento 2 open-source (Community), Magento 2 Commerce (EE), Magento Cloud, Magento B2B, Magento MSI.

- Magento v2.0.x
- Magento v2.1.x
- Magento v2.2.x
- Magento v2.3.x
