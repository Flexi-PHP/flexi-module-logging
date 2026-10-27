# Logging Module

The Logging module provides a PSR-3 logger backed by the Flexi contract log repository and an in-file repository adapter. It also registers an event listener that records dispatched events.

## Configuration

`Config/services.json` registers the `logger` service and `LogRepositoryInterface` adapter. Configure `log_file_path` and `log_format` through the application configuration. `Config/listeners.json` subscribes the logger listener to all events.

Install `flexi/flexi-module-logging` with Composer and activate the `Logging` module. The module supports PHP 7.4+, Flexi Core `^3.2`, and `flexi/contracts` `^5.2.1`.

## Tests

Install the development dependencies with `composer install`, then run `vendor/bin/phpunit tests` from the module root.
