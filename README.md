если потребуется склонировать репозиторий без самых тяжеловесных файлов, которые сейчас в Git LFS ![image](https://github.com/user-attachments/assets/684b8094-9ac8-431c-8ec6-a84ddb998433)

то использовать GIT_LFS_SKIP_SMUDGE=1 git clone https://github.com/victoriaraznodumova/machine-learning-studying-projects.git
тогда LFS-файлы не будут скачаны, но на их месте будут заглушки (~текстовые ссылки на содержимое)

можно скачать только нужные файлы вручную:
git lfs pull --include="пр 5/users.csv"
git lfs pull --include="*.csv"
