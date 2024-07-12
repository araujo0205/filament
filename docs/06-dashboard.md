---
title: Dashboard
---

Filament allows you to build dynamic custom dashboard widgets very easily. To get started building a `Stats` widget:

```bash
php artisan make:filament-widget Stats
```

This command will create two files - a widget class in the `/Widgets` directory of the Filament directory, and a view in the `/widgets` directory of the Filament views directory.

Widgets are pure [Laravel Livewire](https://laravel-livewire.com) components, so may use any features of that package.

> Pre-built widget templates are coming soon. For more information, please see our [Development Roadmap](roadmap).

## Disabling the Default Widgets

By default, two widgets are displayed on the dashboard. These widgets can be disabled by updating the `AdminPanelProvider` file. Remove the lines inside widget function in file `app/Providers/Filament/AdminPanelProvider.php`:

```php
    ->widgets([
        // Widgets\AccountWidget::class,
        // Widgets\FilamentInfoWidget::class,
    ])
```
