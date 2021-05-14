## テーブル設計

## users table - prototypes comments - has_many

| Column     | Type   | Option      |
| ---------- | ------ | ----------- |
| email      | string | null: false |
| password   | string | null: false |
| name       | string | null: false |
| profile    | text   | null: false |
| occupation | text   | null: false |
| position   | text   | null: false |

## prototypes table - comments - has_many

| Column     | Type          | Option      | 
| ---------- | ------------- | ----------- |
| title      | string        | null: false |
| catch_copy | text          | null: false |
| concept    | text          | null: false |
| image      | ActiveStorage |             
| user       | reference     |             

## comments table

| Column    | Type      | Option      | 
| --------- | --------- | ----------- |
| text      | text      | null: false |
| user      | reference |             
| prototype | reference |