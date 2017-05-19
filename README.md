# MyDNSHost bulk importer

This repository contains code to take a directory of zone files and bulk-import their contents into http://www.mydnshost.co.uk/

## Usage:

- Clone the repo
- Grab dependencies via composer `composer update`
- Create config.local.php with your user and API key:
```php
	$config['user'] = 'admin@example.org.uk';
	$config['apikey'] = 'AAAAAAAA-BBBB-CCCC-DDDD-EEEEEEEEEEEE';
```
- Add zone files (ending in `.zone` or `.db`) into the `zones/` directory
- Run the importer with `php run.php`
