## messagesテーブル

|Column|Type|Options|
|------|----|-------|
|body|text||
|image|string||
|user_id|integer|null: false, foreign_key: true|
|group_id|integer|null: false, foreign_key: true|
|timestamps|null: false|

### Association
- belongs_to :group
- belongs_to :user

## usersテーブル

|Column|Type|Option|
|------|----|------|
|name|string|null:false|
|mail|string|null:false|
|password|string|null:false|
||timestamps|null:fasle|

### Association
- has_many :messages
- has_many :group through:members

## groupsテーブル

|Column|Type|Option|
|------|----|------|
|name|string|null:false|
|user_id|integer|null:false, foreign_key: true|

###Association
- has_many :users through: members
- has_many :messages




### index
-add_index :messages [:body,:image]
-add_index :users [:name,:mail,:password]
-add_index :groups [:name]

