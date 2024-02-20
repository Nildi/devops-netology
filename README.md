# devops-netology
Git не будет брать под свой контроль следующие файлы:
<br>*  обозначает любое количество элементов
Локальные каталоги .terraform:
**/.terraform/*

Файлы .tfstate:
*.tfstate
*.tfstate.*

Файлы журналов сбоев:
crash.log
crash.*.log

Все файлы .tfvars:
*.tfvars
*.tfvars.json

Все файлы имеющие расширения:
override.tf
override.tf.json
*_override.tf
*_override.tf.json

Но при этом будут отслеживаться файлы, которые попали под исключения:
!example_override.tf

Так же можно добавить в исключения файлы tfplan, чтобы игнорировать вывод плана команды: terraform plan -out=tfplan
 Пример: *tfplan*

Файлы конфигурации CLI:
.terraformrc
terraform.rc
