## Sample OSGI Project

This is a simple osgi java template based on tycho maven plugin

### How to build

```
mvn verify
```


* Download [Apache felix](https://downloads.apache.org//felix/org.apache.felix.main.distribution-7.0.0.zip)

execute following commands

```
java -jar bin/felix.jar
```

You should see gogo shell

```
install ${PROJECTDIR}/org.omidbiz.user/target/org.omidbiz.user-8.1.0-SNAPSHOT.jar
lb
start ${BUNDLENUMBER}
lb
```
you shoulde see 

```
20|Active     |    1|Omidbiz User Library (8.1.0.202102270445)|8.1.0.202102270445
```

###  How to import into eclipse IDE


Navigate to Window > Preferences
Navigate to Maven > Discovery
Click Open Catalog
On Find field, enter Tycho
Select Tycho Configurator, click Finish to install it
Accept the terms, certificate, etc until installed


import existing maven project
