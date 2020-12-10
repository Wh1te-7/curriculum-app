## usersテーブル

| Column             | Type   | Option   |
| ------------------ | ------ | -------- |
| email              | string | NOT NULL |
| encrypted_password | string | NOT NULL |
| nickname           | string | NOT NULL |
| birthday           | date   | NOT NULL |
| college            | string | NOT NULL |

### Association
 - has_many :users

## Classesテーブル

| Column    | Type       | Option            |
| --------- | ---------- | ----------------- |
| title     | string     | NOT NULL          |
| day_id    | integer    | NOT NULL          |
| number_id | integer    | NOT NULL          |
| teacher   | string     | NOT NULL          |
| text      | text       | NOT NULL          |
| comment   | text       |                   |
| user      | references | foreign_key: true |

### Association
 - belongs_to :user

