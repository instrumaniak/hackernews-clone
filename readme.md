## Hacker news clone

**Backend**: python, django, graphene

Based on this tutorial: https://www.howtographql.com/graphql-python/0-introduction/

The main motivation for doing this tutorial was [Saleor](https://www.saleor.io). I was working on customizing the *Saleor Dashboard* at my job and wanted to get some idea about how the Saleor's Django backed is working.

Here are some of my observations/situations that I faced as I went through the tutorials:

- saleor backend has graphql-playground included. I had included `django-graphql-playground` but then removed it as it was reusing saleor's tabs. As both of the django projects ran on the same ports. So after searching for alternatives, I found [Altair GraphQL Client](https://github.com/imolorhe/altair) chrome extension, it's nice.

- While working with django & python, I realized that how deeply I liked the TypeScript support in the code editor. Athough, vscode python extension provided a lot of suggestions. So, fullstack typescript/javascript setup is much confortable to me.


### Installation

```
cd api/
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```