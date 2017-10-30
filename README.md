# H&O Magento 2 Norsk Bokmål Translations

## Installation through composer
```BASH
composer require honl/magento2-nb-no dev-master
```

## Contributing
Go to <a href="https://crowdin.com/project/magento-2/no#Head">CrowdIn</a> and translate files.

## Import translations:
```BASH
curl http://107.170.242.99/build.php
cd vendor/honl/magento2-nb-no
wget -O crowdin.csv http://107.170.242.99/var/Head/source_no_NO.csv
git commit -am"Imported translations from crowdin"
git push
```

## How are translations files loaded
In the file `Magento\Framework\App\Language\Dictionary::readPackCsv` all ``*.csv` files are loaded, no specific filename
required.

## Credits
This extension was developed by H&O with a lot of help from the Magento Community on CrowdIn. www.h-o.nl
