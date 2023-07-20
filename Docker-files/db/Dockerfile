FROM mysql:8.0.33
LABEL "Project"="Vprofile"
LABEL "Author"="Shariq"

ENV MYSQL_ROOT_PASSWORD="vprodbpass"
ENV MYSQL_DATABASE="accounts"

# Use the db_backup.sql from the vprofile/vprofiledb image
COPY --from=vprofile/vprofiledb:V1 /docker-entrypoint-initdb.d/db_backup.sql /docker-entrypoint-initdb.d/db_backup.sql
