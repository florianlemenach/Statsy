# Server-Stats
PHP Tool to easily get server information

Server-Stas is a group of premade easy to use functions that can return various types of information about your server.

## What information can i get with Server-Stats
With Server-stats you can get the folling information:

- Uptime - (Days, Hours, Mins, Secs)                                                             
- Total RAM - (Ammount in Kilobytes, MegaBytes, Gigabytes)                                  
- Available - RAM (Ammount in Kilobytes, MegaBytes, Gigabytes)                              
- Free RAM - (Ammount in Kilobytes, MegaBytes, Gigabytes)                                   
- Used RAM - (Ammount inKilobytes, MegaBytes, Gigabytes or %)                              
- CPU Useage - (As a %)                                                         
- CPU Info - (model, clock speed, cache ammount, cores)                
- Total Disk - Space (Ammount in Kilobytes, MegaBytes, Gigabytes)                           
- Total Free Disk Space - (Ammount Kilobytes, MegaBytes, Gigabytes)                      
- Disk Space Used - (Ammount Kilobytes, MegaBytes, Gigabytes or %)

##Function Names

Uptime:
```php
get_uptime($arg)
```
Ram:
```php
get_totalram($arg)
get_availableram($arg)
get_freeram($arg)
get_usedram($arg)
get_usedram2()
```

CPU:
```php
get_cpu_usage()
get_cpuinfo($arg)
```

HHD/SSD
```php
get_disktotalspace($arg)
get_diskfreespace($arg)
get_diskusedspace($arg)
get_diskusedspace2()
```

##How To Use
To use Server-Stas just use it as a php include on your project

```php
<?php include_once 'directory/from/file/you/want/to/use/it/on/Server-Stats.php' ?>
```
or

```php
<?php include_once 'directory/from/file/you/want/to/use/it/on/Server-Stats-Dev.php' ?>
```

###Useing Each Function
To use the function just call then whereever you need them, if you wanna echo the number out make sure you use ```php echo ``` before the function call. An example of useing one of the function and adding some text with it would be  ```php echo get_usedram(gb) . ' ' . 'Ram Being Used'; ``` This would show '[yourram] GB Ram Being Used'

####get_totalram($arg)
get_totalram($arg) can be used as follows, kb will return the value in kilobytes, mb will return the value in megabytes and gb will return the value in gigabytes.
```php
get_totalram(kb) 
get_totalram(mb)
get_totalram(gb)
```

####get_availableram($arg)
get_availableram($arg) can be used as follows, kb will return the value in kilobytes, mb will return the value in megabytes and gb will return the value in gigabytes.
```php
get_availableram(kb) 
get_availableram(mb)
get_availableram(gb)
```

####get_freeram($arg)
get_freeram($arg) can be used as follows, kb will return the value in kilobytes, mb will return the value in megabytes and gb will return the value in gigabytes.
```php
get_freeram(kb) 
get_freeram(mb)
get_freeram(gb)
```

####get_usedram($arg)
get_usedram($arg) can be used as follows, kb will return the value in kilobytes, mb will return the value in megabytes and gb will return the value in gigabytes.
```php
get_usedram(kb) 
get_usedram(mb)
get_usedram(gb)
```

####get_usedram2()
get_usedram2() can be used as follows and will return the used ram as a %
```php
get_usedram2() 
```

####get_cpu_usage()
get_cpu_usage() can be used as follows and will return the cpu load as a %
```php
get_cpu_usage()
```

####get_cpuinfo($arg)
get_cpuinfo($arg) can be used as follows, model will return the CPU model, cores will return the ammount of cores the CPU has, speed will return the clock speed, cache will return the CPU cache ammount
```php
get_cpuinfo(model)
get_cpuinfo(cores)
get_cpuinfo(speed)
get_cpuinfo(cache)
```

####get_disktotalspace($arg)
get_disktotalspace($arg) can be used as follows, kb will return the value in kilobytes, mb will return the value in megabytes and gb will return the value in gigabytes.
```php
get_disktotalspace(kb)
get_disktotalspace(mb)
get_disktotalspace(gb)
```

####get_diskfreespace($arg)
get_diskfreespace($arg) can be used as follows, kb will return the value in kilobytes, mb will return the value in megabytes and gb will return the value in gigabytes.
```php
get_diskfreespace(kb)
get_diskfreespace(mb)
get_diskfreespace(gb)
```

####get_diskusedspace($arg)
get_diskusedspace($arg) can be used as follows, kb will return the value in kilobytes, mb will return the value in megabytes and gb will return the value in gigabytes.
```php
get_diskusedspace(kb)
get_diskusedspace(mb)
get_diskusedspace(gb)
```

####get_diskusedspace2()
get_diskusedspace2() can be used as follows and will return the used disk space as a %
```php
get_diskusedspace2() 
```


