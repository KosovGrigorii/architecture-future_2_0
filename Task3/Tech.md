# Техрадар

| Технология                | Кольцо | Квадрат                |
|---------------------------|--------|------------------------|
| Java	                    | Adopt  | Languages & Frameworks |
| Python                    | Adopt  | Languages & Frameworks |
| Go                        | Adopt  | Languages & Frameworks |
| PostgreSQL                | Adopt  | Platforms & Operations |
| MinIO                     | Trial  | Platforms & Operations |
| Nessie                    | Trial  | Platforms & Operations |
| Dremio                    | Trial  | Platforms & Operations |
| Apache Airflow            | Assess | Tools                  |
| Microsoft SQL Server 2008 | Hold   | Platforms & Operations |
| Power Builder             | Hold   | Languages & Frameworks |
| Apache Camel              | Hold   | Tools                  |

Объяснение действий из роадмапа
- в начале запускаем MinIO для S3-совместимого хранилища + разворачиваем apache Iceberg для работы с метой. Это первый шаг по созданию LakeHouse
- подключаем Nessie и Dremio, необходимые для контроля версий и работы с данными в SQL формате
- после того, как предыдущие шаги готовы, можно внедрить Airflow и пустить поток данных в новую систему

