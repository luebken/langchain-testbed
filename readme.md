TODO cleanup and see if you can create at least one query that seems to work


-- https://console.cloud.google.com/bigquery
```sql
select sample_repo_name as repo_name, content as package_json
from bigquery-public-data.github_repos.sample_contents
where sample_path like "%/package.json"
limit 1000
```

https://github.com/langchain-ai/langchain/discussions/6378