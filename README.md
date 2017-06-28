# libhsqldb-java-maven Debian package

Official `libhsqldb-java` Debian package installs only `org.hsqldb:hsqldb` artifact into local maven repo (`/usr/share/maven-repo`), but places `hsqldbutil` jar only in `/usr/share/java`.

The current package simply depends on `libhsqldb-java` and creates necessary symlink and POM file in Debian local Maven repo, so that `org.hsqldb:hsqldbutil:debian` available from it.
