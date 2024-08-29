IMSS PDF
===================

Una extensión de la libreria FPDF con tipografia del IMSS, todos los creditos a los creadores de FPDF

[FPDF Website](http://www.fpdf.org/)

Utiliza FPDF 1.86.



## Instalación

Agrega a tu archivo "__composer.json__" dentro de la sección "__require__" lo siguiente:
```
"imssci/pdf": "dev-main"
```
Luego agrega, en ese mismo archivo, dentro de la sección "__repositories__" lo siguiente:
```
[
    {
        "type": "vcs",
        "url": "https://github.com/imssci/pdf.git"
    }
]
```
Si la sección no existe, entonces creala. Por último agrega esto al autoload, deberia parecerse a esto
```
"autoload": {
        "files": [
            "app/Helpers/verPase.php"
        ],
        "psr-4": {
            "App\\": "app/",
            "Database\\Factories\\": "database/factories/",
            "Database\\Seeders\\": "database/seeders/",
            "IMSSCI\\Pdf\\": "src/"
        }
    }
```

Ahora ejecuta:
```sh
composer update
```
Y Listo

## Uso

En el archivo php donde necesites crear la clase usa

```php
use imssci\pdf;
```

Luego sigue la documentación oficial de FPDF

``` php
$pdf = new pdf();
```
