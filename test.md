## これはマークダウンのテスト用ファイルです
### この下に内容を記載します
- usersテーブル
- user_profilesテーブル

```uml
@startuml
  database project {

    entity users {
      * id<<PK>>
      ----
      * email
      * password
    }

    entity user_profiles {
      * id<<PK>>
      ----
      * user_id<<FK>>
      * name
      * profile_text
    }

    users ||--|| user_profiles
  }
@enduml
```
