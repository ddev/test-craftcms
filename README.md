# test-craftcms
Used by automated tests to test craftcms installation

This repo was created with a `composer create-project` using the techniques at https://docs.ddev.com/en/stable/users/quickstart/#craft-cms

`ddev config --name=testpkgshopware6 --project-type=craftcms --docroot=web`

Ran through the ordinary DDEV Quickstart and copied in `web/happy-brad.jpg`

Database db tarball (not db.sql.gz) was created with
```
ddev export-db --gzip=false --file=.tarballs/db.sql && tar -czf .tarballs/db.sql.tar.gz -C .tarballs db.sql
```

Files tarball was created with
```
cd web/files && tar -czf ../../.tarballs/files.tgz .
```