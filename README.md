# flysystem-cloudinary-adapter

This is quickly done in order to satisfy current needs. My contain a lot of bugs.
I guess this is work in progress.

Since Cloudinary (great service!) has really bad both documentation and official PHP library - making this was a pain.
Hence for now there is no tests.


## Install

Via Composer

## Usage

``` php
$config = [
    'api_key' => env('CLOUDINARY_API_KEY'),
    'api_secret' => env('CLOUDINARY_API_SECRET'),
    'cloud_name' => env('CLOUDINARY_CLOUD_NAME'),
];
$filesystem = new League\Flysystem\Filesystem(new CloudinaryAdapter($config, new Cloudinary\Api));
```

## Contributing

Contributions are **welcome** and will be fully **credited**.

## Credits

- [t3chnik][link-author]
- [All Contributors][link-contributors]

## License

The MIT License (MIT). Please see [License File](LICENSE.md) for more information.

[link-author]: https://github.com/t3chnik
[link-contributors]: ../../contributors
