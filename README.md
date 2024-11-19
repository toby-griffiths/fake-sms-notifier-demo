# Demo of non-dev fake-sms-notifier

Clone this repo, run composer install, then try senign a notificaion using fakesms+email://…

```
$ ./bin/console app:send-fake-sms
```

This doesn't work because symfony/fakse-sms-notifier is installed as a dev requirement.

To fix…

```
$ composer remove --dev symfony/fake-sms-notifier
$ composer require symfony/fake-sms-notifier
```

Then try resending.  Should work.
