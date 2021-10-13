Open and configure install at `https://<your-ip>:443`

Collaborative Editing
Nextcloud's built-in collaborative editing packages (Collabora/CODE and OnlyOffice) only work on x86_64 systems with glibc, and therefore they are not compatible with our images. You should create separate containers for them and set them up in Nextcloud with their respective connector addons.

If (auto) installed, those built-in packages may cause instability and should be removed

Add trusted domains to config/www/config/config.php

```php
  'trusted_domains' => 
  array (
    0 => 'nextcloud.local',
    1 => 'nextcloud.my.domain.com',
    2 => 'localhost'
  ),
```


Install SSL certs from /config/keys/*

## Reference

* [linuxserver/docker-nextcloud](https://github.com/linuxserver/docker-nextcloud)