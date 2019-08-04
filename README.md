# phpUnitTest

#setting up

1. install composer
2. install phunit from composer (composer install phpunit/phpunit)
3. add autolaod in composer.json

    "autoload": {
    	"psr-4": {
    		"App\\": "app"
    	}
    }
    
4. composer dump-autoload
5. add basic phpunit.xml

    <?xml version="1.0" encoding="UTF-8"?>
    <phpunit bootstrap="vendor/autoload.php"
             colors="true"
             verbose="true"
             stopOnFailure="false">
        <testsuites>
            <testsuite name="Tets Suite">
                <directory>tests</directory>
            </testsuite>
        </testsuites>
    </phpunit>
    
  
