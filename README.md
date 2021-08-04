Содержимое файла `.git/hooks/commit-msg`
```shell
#!/bin/bash
message=`cat $1`
php -f commit-msg.php -- "commit-text=${message}"
```

Файл нужно сделать исполняемым ` chmod +x .git/hooks/commit-msg`
