### В соответствии с .gitignore будут исключены:
 1. все файлы подкаталога **.terraform** в каталоге **terraform** 
 2. файлы состояния с расширениями **.tfstate**, **.tfstate.**
 3. файлы журнала сбоев - **crash.log**
 4. все файлы с расширением **.tfvars**, так как они могут содержать секретные данные (пароли, ключи), или данные, которые могут меняться в зависимости от окружения.
 5. проигнорированы файлы **override.tf** и **override.tf.json**, а также файлы, имя которых заканчивается на **_override.tf** и **_override.tf.json**
 6. проигнорированы конфигурационные файлы **.terraformrc**, **terraform.rc**
    
 При необходимости отслеживать файлы, которые попали под исключение, используйте шаблон:
 **!Example_override.tf** 

 Чтобы игнорировать план вывода команды: **terraform plan -out=tfplan**, включите **tfplan** файлы. 
 Например: **tfplan**



