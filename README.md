# server-database-backup

## How to backup?

```
mysqldump -h ~.~.~.rds.amazonaws.com -u admin -p violet --skip-lock-tables  --column-statistics=0 > b.sql

github-release upload \
  --owner project-violet \
  --repo server-database-backup \
  --tag ~ \
  --release-name ~ \
  --body "" \
  --token ~ \
  --prerelease=false \
  violet-~.sql
```
