# Nova Scheduled Jobs

## Includes both a tool and card to display your scheduled commands and jobs


## Installation

You can install the package in to a Laravel app that uses [Nova](https://nova.laravel.com) via composer:

```bash
composer require llaski/nova-scheduled-jobs
```

To setup the tool, you must register the tool with Nova. This is typically done in the `tools` method of the `NovaServiceProvider`.

```php
// in app/Providers/NovaServiceProvider.php

// ...

public function tools()
{
    return [
        // ...
        new \Llaski\NovaScheduledJobs\NovaScheduledJobsTool,
    ];
}
```

To setup the card, you must register the card with Nova. This is typically done in the `cards` method of the `NovaServiceProvider`.

```php
// in app/Providers/NovaServiceProvider.php

// ...

public function cards()
{
    return [
        // ...
        new \Llaski\NovaScheduledJobs\NovaScheduledJobsCard,
    ];
}
```

### Testing

``` bash
phpunit
```

## License

The MIT License (MIT). Please see [License File](LICENSE.md) for more information.
