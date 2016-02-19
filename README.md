# xmlsec v1.5.8 with replaced commons-logging dependency with java-util logging
modified version of Apache XML Security that does not contain any commons-logging dependency. commons-logging is replaced with java-util logging. The real reason behind is that classes of xmlsec is being bundled with webservices-osgi artefact of Metro as of version 2.3.2-b607. This introduces commons-logging dependency to OSGI containers, such as Glassfish, when regarding Metro version is used. commons-logging is not OSGi friendly (see http://wiki.apache.org/commons/CommonsOsgi) due to the classloader work that it implements.

THe 1.5.8 version of xmlsec is used.
