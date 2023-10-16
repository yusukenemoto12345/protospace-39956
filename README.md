# README

# テーブル設計	
	
## users テーブル	
	
| Column | Type | Options |	
| ------------------ | ------ | ----------- |	
| name | string | null: false |	
| email | string | null: false |	
| encrypted_password | string | null: false |	
| occupation | text | null: false |	
| profile | text | null: false |	
| position | text | null: false |	
	
	
## prototypes テーブル	
	
| Column | Type | Options |	
| ------------------ | ------ | ----------- |	
| title | string | null: false |	
| catch_copy | text | null: false |	
| concept | text | null: false |	
| user | references | null: false, foreign_key: true |	
	
## comments テーブル	
	
| Column | Type | Options |	
| ------------------ | ------ | ----------- |	
| content | text | null: false |	
| prototype | references | null: false, foreign_key: true |	
| user | references | null: false, foreign_key: true |	
	
