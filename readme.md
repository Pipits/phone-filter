# Phone template filter

This is a Perch template filter for formatting phone numbers.


## installation
- Download the latest version
- Place the `pipit_phone` directory in the folder `perch/addons/templates/filters/`
- Include the class in the file `perch/addons/templates/filters.php`:

```php
include('filters/pipit_phone/PipitTemplateFilter_phone.class.php');
```


## Configuration

### Enable template filters

You need to enable template filters in your config file `perch/config/config.php`:

```php
define('PERCH_TEMPLATE_FILTERS', true);
```

### Set a default country [optional]

You can set a default country to format the numbers to its standards:

```php
define('PIPIT_PHONE_COUNTRY', 'GB');
```



## Usage

```html
<a href="<perch:content id="phone_number" filter="phone" output="tel_link">" >
    <perch:content id="phone_number" filter="phone" output="international">
</a>
```
