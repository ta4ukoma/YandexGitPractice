# This is training git for practice on yandex practicum

### HESH
Хэш сумма - это число-буквенная  последовательность коммита, является уникальной последовательностью и однозначно определяет один только коммит.

### git log
Данная команда позволяет просматривать все коммиты репозитория и на основании хэш суммы понимать что было сделано и в какой момент времени произошли те или иные изменения в репозитории.

### HEAD
HEAD — это указатель на текущую ветку, которая, в свою очередь, является указателем на последний коммит, сделанный в этой ветке. Это значит, что HEAD будет родителем следующего созданного коммита. Как правило, самое простое считать HEAD снимком вашего последнего коммита. В папке .git есть файл с аналогичным названием где записывается hesh summ последнего коммита.

### git status
Крайне важная команда, кторой стоит пользоваться перед любыми действиями в репозитории. Она покажет в какой ветке вы находитесь и статусы файлов в репозитории.

### git commit markdown
очень важно оформлять коммиты в соответствии с той практикой, которая принята в команде остальными разработчиками. Я вот даже в своем репозитории учебном забыл это сделать. Мне следовало оформлять каждый коммит указанием того какой файл был изменен.

### Life circle of git

```mermaid
graph LR;
    A["WorkDir(Untracked by Git)"] -- git init --> B["WorkDir(Tracked by GIT)"];
    B["WorkDir(Tracked by GIT)"] -- git add --> C[Staging Area];
    C[Staging Area] -- git commit --> D[Local repository];
    D[Local repository] -- git push --> E[Remote repository];

```

### ToDo
1. For begin open the Terminal app and type command - git init, do it in right folder.
2. Make you files by command - touch.
3. Every step you need to commit - git add . && git commit -m "type something right".
4. Link local git and remote git - git remote add origin git@github.com:yourname/yourrepo
5. PROFIT =)
