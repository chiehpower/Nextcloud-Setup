# Disable the slogan - “Get your own free account”

Add this in /path/to/nextcloud/config/config.php

```
'simpleSignUpLink.shown' => false,
```

In my case, I was using the docker container way to start the nextcloud, so I have to access into this container.
For example:

```
root@d5ddf0987fb0:/var/www/html# vim config/config.php 
root@d5ddf0987fb0:/var/www/html# cat config/config.php 
<SKIP>
  'app_install_overwrite' => 
  array (
    0 => 'files_downloadactivity',
    1 => 'files_trackdownloads',
    2 => 'workflow_pdf_converter',
  ),
  'simpleSignUpLink.shown' => false,
);
```

# Reference:
- https://help.nextcloud.com/t/remove-link-get-your-own-free-account/41131