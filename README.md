## usersテーブル

email  (string, NOT NULL, ユニーク制約)
encrypted_password  (string,  NOY NULL)
name  (string, NOT NULL)
profile  (text, NOT NULL)
occupation  (text, NOT NULL)
position  (text, NOT NULL)


## prototypesテーブル

title  (string, NOT NULL)
catch_copy  (text, NOT NULL)
concept  (text, NOT NULL)
user  (references, NOT NULL)


## commentsテーブル

content  (text, NOT NULL)
prototype  (references, NOT NULL, 外部キー)
user  (references, NOT NULL, 外部キー)
