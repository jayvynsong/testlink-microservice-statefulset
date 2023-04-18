# testlink-microservice-statefulset
Build Testlink integrated enviroments based on microservice with StatefulSet. K8S, Jenkins and other DevOps tools will be integrated in future.

## Environment Variables

### Database

* `DATABASE_USER`: The user to use for connecting to the TestLink database (default: root)
* `DATABASE_PASS`: The password to use for connecting to the TestLink database (default: testlink)
* `DATABASE_HOST`: The host to use when connecting to the TestLink database (default: testlink-db-service)
* `DATABASE_NAME`: The name of the database that contains the TestLink tables (default: testlink)

### SMTP

* `SMTP_HOST`: The SMTP host (the email server)
* `SMTP_ADMIN_EMAIL`: The email that problem/error notifications will be sent to
* `SMTP_FROM_EMAIL`: The email that all emails will be sent by
* `SMTP_RETURN_PATH`: The "Reply-To" email of all emails sent
* `SMTP_PRIORITY`: Priority of email - Urgent = 1, Not Urgent = 5, Disable = 0
* `SMTP_USERNAME`: Username to authenticate against the SMTP server
* `SMTP_PASSWORD`: Password to authenticate against the SMTP server

### Path

* `LOG_PATH`: The location of the logs (default: /var/testlink/logs/)
* `UPLOAD_PATH`: The location of the uploads (default: /var/testlink/upload_area/)

### Misc

* `DEBUG_ON`: Set to `1` to enable ALWAYS dBug()
* `TEXT_EDITOR`: Which text editor you'd like to use (non-default options: tinymce, or none)
* `LOG_LEVEL`: NONE, ERROR, INFO, DEBUG, EXTENDED
* `ENABLE_TEST_AUTOMATION`: ENABLED, DISABLED
