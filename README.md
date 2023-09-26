# DB 設計

## users table

| Column             | Type        | Options                        |
|--------------------|-------------|--------------------------------|
| employee_number    | string      | null: false, unique: true      |
| encrypted_password | string      | null: false                    |
| last_name_kanji    | string      | null: false                    |
| first_name_kanji   | string      | null: false                    |
| last_name_kana     | string      | null: false                    |
| first_name_kana    | string      | null: false                    |
| phone_number       | string      | null: false                    |

### Association
- has_many :
- has_many :
- has_many :



## departments table

| Column                               | Type         | Options                        |
|--------------------------------------|--------------|--------------------------------|
| user                                 | references   | null: false, foreign_key: true |
| department_name                      | string       | null: false                    |
| department_detail                    | text         | null: false                    |
| department_assignee_last_name_kanji  | string       | null: false                    |
| department_assignee_first_name_kanji | string       | null: false                    |
| start_date                           | date         | null: false                    |
| end_date                             | date         | null: false                    |

### Association
- has_many :
- belongs_to :



## divisions table

| Column                             | Type         | Options                        |
|------------------------------------|--------------|--------------------------------|
| user                               | references   | null: false, foreign_key: true |
| department                         | references   | null: false, foreign_key: true |
| division_title                     | string       | null: false                    |
| division_detail                    | text         | null: false                    |
| division_assignee_last_name_kanji  | string       | null: false                    |
| division_assignee_first_name_kanji | string       | null: false                    |
| status                             | integer      | null: false                    |

### Association
- has_many :
- belongs_to :



## tasks table

| Column           | Type          | Options                         |
|------------------|---------------|---------------------------------|
| content          | string        | null: false                     |
| pr| integer       |                                 |
| im   | integer       |                                 |

### Association

- belongs_to :
- belongs_to :