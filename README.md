# mrg1790_platform
mrg1790 Platform repository
Выполнено:
 task01:
 - Создать Service Account bob , дать ему роль admin в рамках всего кластера
 - Создать Service Account dave без доступа к кластеру
 task02:
 - Создать Namespace prometheus
 - Создать Service Account carol в этом Namespace
 - Дать всем Service Account в Namespace prometheus возможность делать
 - get , list , watch в отношении Pods всего кластера
 task03:
 - Создать Namespace dev
 - Создать Service Account jane в Namespace dev
 - Дать jane роль admin в рамках Namespace devmkdir
 - Создать Service Account ken в Namespace dev
 - Дать ken роль view в рамках Namespace dev