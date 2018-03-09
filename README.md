# Прим: здесь и далее не забывайте заменять user на ваше имя в GitHub,
# а repository на имя вашего репозитория.

# Клонируем наш репозиторий в локальную папку:
git clone github.com/user/repository.git

# Создаем ветку gh-pages
cd repository
git checkout --orphan gh-pages

# Удаляем всё лишнее
git rm -rf .

# Создаём и коммитим index.html
echo "Test" > index.html
git add index.html
git commit -a -m "Testing gh-pages"

# Закидываем изменения обратно на GitHub
git push origin gh-pages
