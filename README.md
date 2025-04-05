# Домашнее задание к занятию "`GitLab`" - `Inshakov Vladimir`

### Задание 1

Что нужно сделать:

    Разверните GitLab локально, используя Vagrantfile и инструкцию, описанные в этом репозитории.
    Создайте новый проект и пустой репозиторий в нём.
    Зарегистрируйте gitlab-runner для этого проекта и запустите его в режиме Docker. Раннер можно регистрировать и запускать на той же виртуальной машине, на которой запущен GitLab.

В качестве ответа в репозиторий шаблона с решением добавьте скриншоты с настройками раннера в проекте.


![Screen_1_1](https://github.com/MrVanG0gh/Netology-8.3-GitLab-hw/blob/main/images/Screenshot_ex1_1.png)
![Screen_1_2](https://github.com/MrVanG0gh/Netology-8.3-GitLab-hw/blob/main/images/Screenshot_ex1_2.png)
![Screen_1_3](https://github.com/MrVanG0gh/Netology-8.3-GitLab-hw/blob/main/images/Screenshot_ex1_3.png)
![Screen_1_4](https://github.com/MrVanG0gh/Netology-8.3-GitLab-hw/blob/main/images/Screenshot_ex1_4.png)

Настройки раннера из файла config.toml:
```
concurrent = 1
check_interval = 0
shutdown_timeout = 0

[session_server]
  session_timeout = 1800

[[runners]]
  name = "neto-runner"
  url = "http://localhost/"
  id = 1
  token = "t3_UhumJ4yHmgozkzsf-eWS"
  token_obtained_at = 2025-04-05T21:09:52Z
  token_expires_at = 0001-01-01T00:00:00Z
  executor = "docker"
  [runners.cache]
    MaxUploadedArchiveSize = 0
    [runners.cache.s3]
    [runners.cache.gcs]
    [runners.cache.azure]
  [runners.docker]
    tls_verify = false
    image = "golang 1.17"
    privileged = false
    disable_entrypoint_overwrite = false
    oom_kill_disable = false
    disable_cache = false
    volumes = ["/cache"]
    shm_size = 0
    network_mtu = 0
```

---

### Задание 2

Задание 2

Что нужно сделать:

    Запушьте репозиторий на GitLab, изменив origin. Это изучалось на занятии по Git.
    Создайте .gitlab-ci.yml, описав в нём все необходимые, на ваш взгляд, этапы.

В качестве ответа в шаблон с решением добавьте:

    файл gitlab-ci.yml для своего проекта или вставьте код в соответствующее поле в шаблоне;
    скриншоты с успешно собранными сборками.


```
Поле для вставки кода...
....
....
....
....
```

`При необходимости прикрепитe сюда скриншоты
![Название скриншота 2](ссылка на скриншот 2)`


---
