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

### Association
- has_many :members
- has_many :messages
- has_many :group through:members

## groupsテーブル

|Column|Type|Option|
|------|----|------|
|name|string|null:false,unique: true|

### Association
- has_many: members
- has_many :users through: members
- has_many :messages

## membersテーブル

|Column|Type|Option|
|------|----|------|
|group_id|integer|foreign_key: true|
|user_id|integer|foreign_key: true|

### Association
- belongs_to :group
- belongs_to :message

## index
- add_index :messages [:body,:image]
- add_index :users [:name,:mail,:password]
- add_index :groups [:name]

