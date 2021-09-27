# data-copier
 data pipeline in python

1. Set up
   ```
    $ pip install pandas
    $ pip install mysql-connector-python
    $ pip install psycopg2-binary
    ```
- check installed version
```
    $ pip freeze
```
- then write into requirements.txt

- read os level implementation eg
```
   $ export SOURCE_DB_USER=retail_user
```
- ls -altr and add gitignore to add files not needed 
- use version control; git init, git add . , git commit -m "message", git push

```buildoutcfg
>>> tables_to_be_loaded=pd.read_csv('table_list',sep=':')
>>> tables_to_be_loaded
    table_name to_be_loaded
0    customers          yes
1  departments          yes
2   categories          yes
3     products          yes
4       orders          yes
5  order_items          yes
>>> tables_to_be_loaded.query("to_be_loaded=='yes'")
    table_name to_be_loaded
0    customers          yes
1  departments          yes
2   categories          yes
3     products          yes
4       orders          yes
5  order_items          yes

```
