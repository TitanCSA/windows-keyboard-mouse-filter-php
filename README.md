# Windows-Keyboard-Mouse-Filter PHP SDK

> [!IMPORTANT]
> **Get the driver without the one-hour demo limit**
>
> On [Discord](https://discord.com/app), choose **Friends → Add Friend**, enter **`titancsa`** and send the project name. Ask about the full **Windows Keyboard Mouse Filter** driver for this SDK. TitanCSA shares purchase details privately.

`composer require titancsa/windows-keyboard-mouse-filter`

PHP 8.2+ Windows x64, extension FFI and `ffi.enable=true` are required. Matching driver installed separately; licensing and trial rules remain unchanged. Supported families: keyboard, mouse.

```php
require "vendor/autoload.php";
$client = new \TitanCSA\Products\WindowsKeyboardMouseFilter\Interceptor();
try { print_r($client->info()); } finally { $client->close(); }
```

See [API](docs/API.md). Installation and construction do not start input capture.
