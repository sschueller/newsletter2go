##newsletter2go
=============

Composer PHP package for https://www.newsletter2go.de/ API


##Usage

####composer.json
```
    "repositories": [
        {
            "type": "package",
            "package": {
                "name": "sschueller/newsletter2go",
                "version": "dev-master",
                "source": {
                    "url": "git://github.com/sschueller/newsletter2go.git",
                    "type": "git",
                    "reference": "master"
                },
                "autoload": {
                    "psr-0" : {
                        "sschueller\\newsletter2go" : "src"
                    }
                }
            }
        }
    ]
```

####In code
```
    // newsletter2go
    $n2go = new \sschueller\newsletter2go\newsletter2go('API KEY');
    $n2go->createRecipient('someemail@domain.com', '+12345678901', array(
        'firstname' => 'John',
        'lastname' => 'Doe',
        'gender' => 'm'
    ));

```