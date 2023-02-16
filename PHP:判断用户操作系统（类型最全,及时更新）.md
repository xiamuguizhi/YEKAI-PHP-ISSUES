```php
<?php
    $agent = $_SERVER['HTTP_USER_AGENT'];
    $os = false;
    if(preg_match('/win/i', $agent) && preg_match('/nt 10.0/i', $agent)){
        $os = 'Windows 10';
    }else if (preg_match('/win/i', $agent) && preg_match('/nt 6.2/i', $agent)){
        $os = 'Windows 8';
    }else if (preg_match('/win/i', $agent) && preg_match('/nt 6.1/i', $agent)){
        $os = 'Windows 7';
    }else if (preg_match('/win/i', $agent) && preg_match('/nt 6.0/i', $agent)){
        $os = 'Windows Vista';
    }else if (preg_match('/win/i', $agent) && preg_match('/nt 5.1/i', $agent)){
        $os = 'Windows XP';
    }else if (preg_match('/win 9x/i', $agent) && strpos($agent, '4.90')){
        $os = 'Windows ME';
    }else if (preg_match('/win/i', $agent) && preg_match('/98/i', $agent)){
        $os = 'Windows 98';
    }else if (preg_match('/win/i', $agent) && strpos($agent, '95')){
        $os = 'Windows 95';
    }else if (preg_match('/win/i', $agent) && preg_match('/nt 5/i', $agent)){
        $os = 'Windows 2000';
    }else if (preg_match('/win/i', $agent) && preg_match('/nt/i', $agent)){
        $os = 'Windows NT';
    }else if (preg_match('/win/i', $agent) && preg_match('/32/i', $agent)){
        $os = 'Windows 32';
    }else if (preg_match('/linux/i', $agent) && preg_match('/android 12/i', $agent)){
        $os = 'Android 12';
    }else if (preg_match('/linux/i', $agent) && preg_match('/android 11/i', $agent)){
        $os = 'Android 11';
    }else if (preg_match('/linux/i', $agent) && preg_match('/android 10/i', $agent)){
        $os = 'Android 10';
    }else if (preg_match('/linux/i', $agent) && preg_match('/android q/i', $agent)){
        $os = 'Android Q';
    }else if (preg_match('/linux/i', $agent) && preg_match('/android 9/i', $agent)){
        $os = 'Android 9';
    }else if (preg_match('/linux/i', $agent) && preg_match('/android 7/i', $agent)){
        $os = 'Android 7';
    }else if (preg_match('/linux/i', $agent) && preg_match('/android 6/i', $agent)){
        $os = 'Android 6';
    }else if (preg_match('/linux/i', $agent) && preg_match('/android 5/i', $agent)){
        $os = 'Android 5';
    }else if (preg_match('/linux/i', $agent) && preg_match('/android 4/i', $agent)){
        $os = 'Android 4';
    }else if (preg_match('/linux/i', $agent) && preg_match('/android/i', $agent)){
        $os = 'Android';
    }else if (preg_match('/harmony/i', $agent) && preg_match('/harmony/i', $agent)){
        $os = 'Harmony OS 鸿蒙';
    }else if (preg_match('/linux/i', $agent)){
        $os = 'Linux';
    }else if (preg_match('/unix/i', $agent)){
        $os = 'Unix';
    }else if (preg_match('/sun/i', $agent) && preg_match('/os/i', $agent)){
        $os = 'SunOS';
    }else if (preg_match('/ibm/i', $agent) && preg_match('/os/i', $agent)){
        $os = 'IBM OS/2';
    }else if (preg_match('/Mac/i', $agent) && preg_match('/PC/i', $agent)){
        $os = 'Macintosh';
    }else if (preg_match('/PowerPC/i', $agent)){
        $os = 'PowerPC';
    }else if (preg_match('/AIX/i', $agent)){
        $os = 'AIX';
    }else if (preg_match('/HPUX/i', $agent)){
        $os = 'HPUX';
    }else if (preg_match('/NetBSD/i', $agent)){
        $os = 'NetBSD';
    }else if (preg_match('/BSD/i', $agent)){
        $os = 'BSD';
    }else if (preg_match('/OSF1/i', $agent)){
        $os = 'OSF1';
    }else if (preg_match('/IRIX/i', $agent)){
        $os = 'IRIX';
    }else if (preg_match('/FreeBSD/i', $agent)){
        $os = 'FreeBSD';
    }else if (preg_match('/teleport/i', $agent)){
        $os = 'teleport';
    }else if (preg_match('/flashget/i', $agent)){
        $os = 'flashget';
    }else if (preg_match('/webzip/i', $agent)){
        $os = 'webzip';
    }else if (preg_match('/offline/i', $agent)){
        $os = 'offline';
    }else{
        $os = '根据UserAgent信息自行判断&UserAgent='.$agent;
    }
echo $os;
```
