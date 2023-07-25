# How to use
```shell
npm i
# make sure you are in virtual env
pip install -r requirements.txt

npm run dev # for tailwind compiler
py manage.py makemigrations
py manage.py migrate
py manage.py runserver
```

# Why is there package.json
Tailwind is a big CSS library, so it uses a compiler to check where the styles are being used (.html) and adds JUST the classes we use in the CSS output file. Then we can just include that in our django base template, just like any other CSS file. 
