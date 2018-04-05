---

copyright:
  years: 2015, 2018
lastupdated: "2018-03-16"

---

{:new_window: target="_blank"}
{:codeblock: .codeblock}

# Latest Updates to the Liberty buildpack
{: #latest_updates}

## A list of the latest updates in the Liberty buildpack.

### March 16, 2018: Updated Liberty buildpack v3.19-20180313-1017
* The default Liberty runtime version was updated to the 18.0.0.1 release
* The monthly Liberty runtime version was updated to 2018.3.0.0.
* The IBM JRE version was updated to 8 SR5 FP10
* The IBM JRE version 7 was removed.  
* The DB2 JDBC driver was updated to the `4.23.42` version.

### February 13, 2018: Updated Liberty buildpack v3.18-20180213-1234.
* The monthly Liberty runtime version was updated to 2018.2.0.0.
* The default Liberty runtime also includes the [PI90804 Apache Commons iFix]( http://www-01.ibm.com/support/docview.wss?uid=swg22011428).

### January 31, 2018: Updated Liberty buildpack v3.17.1-20180131-1532.
* The buildpack was updated to include Liberty feature microProfile-1.2. 

### January 26, 2018: Updated Liberty buildpack v3.17-20180122-1037
* The buildpack was updated to add the ability to dynamically set tracing on the Liberty server. 
* The monthly Liberty runtime version was updated to 2018.1.0.0.
* The IBM JRE version was updated to 8 SR5 FP7.

### January 5, 2018: Updated Liberty buildpack v3.16-20180102-0938
* The default Liberty runtime version was updated to the 17.0.0.4 release
* The monthly Liberty runtime version was updated to 2017.12.0.0.
* The IBM JRE version was updated to 8 SR5 FP6.


### October 31, 2017: Updated Liberty buildpack v3.15.
* The monthly Liberty runtime version was updated to 2017.10.0.0.

### October 17, 2017: Updated Liberty buildpack v3.14-20171013-1023
* The default Liberty runtime version wasupdated to the 17.0.0.3 release.
* The monthly Liberty runtime version was updated to 2017.9.0.1.
* The IBM JRE version was updated to 8 SR5.

### October 5, 2017: Updated Liberty buildpack v3.13-20170919-1721
* The monthly Liberty runtime version was updated to 2017.9.0.0.
* The IBM JRE version was updated to 8 SR4 FP11.
* The auto-scaling agent was updated.

### August 14, 2017: Updated Liberty buildpack v3.12-20170814-1322
* The monthly Liberty runtime version was updated to the [2017.8.0.0](https://developer.ibm.com/wasdev/blog/2017/08/04/beta-websphere-liberty-tools-august-2017/) release.
* The buildpack also contains updated IBM JREs: version 8 SR4 FP10 and version 7.1 SR4 FP10.
* JRE 8 includes Java Cryptography Extension (JCE) Unlimited Strength Jurisdiction Policy Files.
* A buildpack bug that prevented Liberty apps from [shutting down gracefully](https://docs.cloudfoundry.org/devguide/deploy-apps/app-lifecycle.html#shutdown) was fixed.

### July 14, 2017: Updated Liberty buildpack v3.11-20170710-0312
* The default Liberty runtime version `17.0.0.2` was updated to include the IFPI83713 iFix.
* The monthly Liberty runtime version was updated to the [2017.7.0.0](https://developer.ibm.com/wasdev/blog/2017/07/07/beta-websphere-liberty-tools-july-2017/) release.
* The buildpack also contains updated IBM JREs: version 8 SR4 FP7 and version 7.1 SR4 FP5.
* The default Cloudant Library is now the official [java-cloudant](https://github.com/cloudant/java-cloudant), the [Ektorp library](https://github.com/helun/Ektorp) is still available as an option, for details on this change see the [blog post](https://www.ibm.com/blogs/bluemix/2017/05/default-library-change-cloudant-auto-wiring-liberty-buildpack/).
* The default heap size ratio is now 50% when your application has less than 512mb of memory, if it has more than 512mb it will still be 75%.
* A new staging task log is now generated, which allows for easier debugging of staging errors.
* The Node.js runtime that is used by the [App Management utility](/docs/manageapps/app_mng.html) was updated to the 6.13.0 version.
* The buildpack also provides an updated agent for the [Auto-Scaling service](/docs/services/Auto-Scaling/index.html).

### June 12, 2017: Updated Liberty buildpack v3.10-20170525-1107
* The default Liberty runtime version was updated to the 17.0.0.2 release.
* The monthly Liberty runtime version was updated to the [2017.5.0.0](https://developer.ibm.com/wasdev/blog/2017/05/12/beta-websphere-liberty-tools-may-2017/) release.
* The Node.js runtime that is used by the [App Management utility](/docs/manageapps/app_mng.html) was updated to the 6.10.0 version.
* The buildpack also provides an updated version of the Extreme Scale Client.

### April 27, 2017: Updated Liberty buildpack v3.9-20170419-1403
* The default Liberty runtime version `17.0.0.1` was updated to include [PI77770](http://www-01.ibm.com/support/docview.wss?uid=swg24043596), [PI77605](http://www-01.ibm.com/support/docview.wss?uid=swg1PI77605), [PI79275](http://www-01.ibm.com/support/docview.wss?uid=swg1PI79275), and PI77438 iFixes.
* The monthly Liberty runtime version was updated to the [2017.3.0.0](https://developer.ibm.com/wasdev/blog/2017/03/14/beta-websphere-liberty-tools-march-2017/) release.
* Memory Calculation was moved from staging to the start process, allowing for easier heap memory changes with the restart of an application.
* The buildpack also provides updated versions of the agent for the [Auto-Scaling service](/docs/services/Auto-Scaling/index.html), and Extreme Scale Client.

### March 14, 2017: Updated Liberty buildpack v3.8-20170308-1507
* The default Liberty runtime version was updated to the 17.0.0.1 release.
* The default Liberty runtime also includes the PI75512 WebSockets iFix.
* The monthly Liberty runtime version was updated to the [2017.2.0.0](https://developer.ibm.com/wasdev/blog/2017/02/17/beta-websphere-liberty-tools-february-2017/) release.
* The IBM JRE versions 8 and 7.1 were updated to SR4 FP1.
* The auto-configuration support was also extended to work with [ibm-websphere-extreme-scale IBM Container](https://console.ng.bluemix.net/docs/images/docker_image_extreme_scale/ibm-websphere-extreme-scale_starter.html).
* The auto-configuration support for [Cloudant NoSQL Database](https://console.ng.bluemix.net/docs/services/Cloudant/index.html) was updated to provide the option of using the Cloudant Java Library instead of org.ektorp. To enable the use of the Cloudant Java Library you must set the following environment variable:    
```
cf set-env <appName> LBP_SERVICE_CONFIG_CLOUDANTNOSQLDB 'type : cloudant'
```
* The buildpack also provides an updated version of the agent for the [Auto-Scaling service](/docs/services/Auto-Scaling/index.html) and a number of application management enhancements.
* This buildpack also changes the way auto-configuration works for the [Monitoring and Analytics service](/docs/services/monana/index.html). Applications using the Free plan will no longer have the log capability added to their applications; it is being replaced by logmet.  


### January 23, 2017: Updated Liberty buildpack v3.7-20170118-2046
* The monthly Liberty runtime version was updated to the [2017.1.0.0](https://developer.ibm.com/wasdev/blog/2017/01/20/beta-websphere-liberty-tools-january-2017/) release.
* The IBM JRE version 8 was updated to SR3 FP22 version.
* The [auto-configuration](autoConfig.html) support was also extended to work with the [Compose for MongoDB service](https://console.ng.bluemix.net/docs/services/ComposeForMongoDB/index.html) (Currently only available with the monthly Liberty runtime).

### December 13, 2016: Updated Liberty buildpack v3.6-20161209-1351
* The default Liberty runtime version was updated to the [16.0.0.4](http://www-01.ibm.com/support/docview.wss?uid=swg27009661) release.
* The IBM JRE version 8 was updated to SR3 FP21 version.
* The [auto-configuration](autoConfig.html) support was also extended to work with the [Compose for PostgreSQL service](https://console.ng.bluemix.net/docs/services/ComposeForPostgreSQL/index.html).
* The buildpack also provides an updated version of the agent for the [Auto-Scaling service](/docs/services/Auto-Scaling/index.html).
* The buildpack was updated to support environment variables as part of the include locations in the `server.xml` files.

### November 29, 2016: Updated Liberty buildpack v3.5-20161114-1152
* The default Liberty runtime version `16.0.0.3` was updated to include [PI62375](https://www-01.ibm.com/support/docview.wss?uid=swg24042712) iFix and to provide the `microProfile-1.0` convenience feature.
* The monthly Liberty runtime version was updated to the `2016.11.0.0` release.
* The buildpack also contains updated IBM JREs: version 8 SR3 FP20 and version 7.1 SR3 FP60.
* The DB2 JDBC driver was updated to the `4.21.29` version.
* The Monitoring and Analytics service integration was fixed to work with [Diego ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://docs.cloudfoundry.org/concepts/diego/diego-architecture.html).
* The [Dynatrace](dynatrace.html) service integrations were updated to work better with the Dynatrace service offerings.
* The [auto-configuration](autoConfig.html) support for PostgreSQL and MySQL type of services was improved to work better when deploying a server directory or packaged server.
* The Node.js runtime that is used by the [devconsole and shell App Management utilities](/docs/manageapps/app_mng.html#app_management) was updated to the latest `0.12.17` version.
* [Security fixes](http://www.ibm.com/support/docview.wss?uid=swg21994945) for the Liberty runtime are included.

### November 1, 2016: Updated Liberty buildpack v3.4.1-20161030-2241
* The buildpack contains a fix for a problem starting certain types of applications. Specifically, applications deployed as a server directory or a packaged server with the application files in the `dropins` directory.

### October 21, 2016: Updated Liberty buildpack v3.4-20161018-2004
* The default Liberty runtime version `16.0.0.3` was updated to include [PI68805](http://www-01.ibm.com/support/docview.wss?uid=swg1PI68805) and [PI69141](http://www-01.ibm.com/support/docview.wss?uid=swg1PI69141) iFixes.
* The monthly Liberty runtime version was updated to the [2016.9.0.1](https://developer.ibm.com/wasdev/blog/2016/09/23/beta-websphere-liberty-and-tools-october-2016/) release.
* The buildpack also contains an updated version of IBM JRE 8.0: SR3 FP12.
* The IBM JRE 8.0 and 7.1 are now configured to enable [all TLS protocols when `SSLContext.getContext("TLS")` is called](https://www.ibm.com/support/knowledgecenter/SSYKE2_8.0.0/com.ibm.java.security.component.80.doc/security-component/jsse2Docs/matchsslcontext_tls.html) to match Oracle's JRE behavior. IBM JRE 7.1 is also configured to enable [all TLS protocols when `SSLContext.getDefault()` is called](https://www.ibm.com/support/knowledgecenter/SSYKE2_7.1.0/com.ibm.java.security.component.71.doc/security-component/jsse2Docs/overrideSSLprotocol.html) to match IBM's JRE 8.0 behavior.
* The buildpack provides an updated data collector for the [Monitoring and Analytics service](/docs/services/monana/index.html#monana_oview).
* The buildpack was changed back to download the latest 1.5.x [MariaDB Connector/J JDBC driver ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://mariadb.com/kb/en/mariadb/about-mariadb-connector-j/) when performing [auto-configuration for MySQL type of services](autoConfig.html).
* The buildpack introduces support for customizing service auto-configuration behavior via the `LBP_SERVICE_CONFIG_<serviceType>` environment variable. For example, it can be used to change the location or version of a JDBC driver to download for the MySQL service. See the documentation of [services that support auto-configuration](autoConfig.html) for more information.
* The buildpack also contains a number of [Diego ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://docs.cloudfoundry.org/concepts/diego/diego-architecture.html) improvements related to application health check and the [App Management](/docs/manageapps/app_mng.html) functionality.

### September 16, 2016: Updated Liberty buildpack v3.3-20160912-1729
* The default Liberty runtime version was updated to the [16.0.0.3](http://www-01.ibm.com/support/docview.wss?uid=swg27009661) release. The monthly Liberty runtime version was updated to the [2016.9.0.0](https://developer.ibm.com/wasdev/blog/2016/08/26/beta-websphere-liberty-and-tools-september-2016/) release. With these updates, the `cloudant-1.0` and `passwordUtilities-1.0` Liberty features, previously available as beta features, are now available as production-ready features.
* [Security fixes](http://www-01.ibm.com/support/docview.wss?uid=swg21990527) for the Liberty runtime are included.
* The buildpack also contains an updated version of IBM JRE 8.0: SR3 FP11.
* The buildpack was adjusted to download the latest 1.4.x [MariaDB Connector/J JDBC driver ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://mariadb.com/kb/en/mariadb/about-mariadb-connector-j/) when performing [auto-configuration for MySQL type of services](autoConfig.html) due to a problem with the latest 1.5.x driver.

### August 26, 2016: Updated Liberty buildpack v3.2-20160822-2200
* The buildpack contains updated versions of IBM JRE: 8 SR3 FP10 and 7.1 SR3 FP50.
* The monthly Liberty runtime version was updated to the [2016.8.0.0](https://developer.ibm.com/wasdev/blog/2016/07/28/beta-websphere-liberty-and-tools-august-2016/) release.
* The service plug-in that provides [auto-configuration support](autoConfig.html) for the [SQL Database](/docs/services/SQLDB/index.html#SQLDB) service was updated to always use the JVM's trusted certificates when connecting to the service over TLS.

### July 22, 2016: Updated Liberty buildpack v3.1-20160717-2254
* The [App Management](/docs/manageapps/app_mng.html) functionality was updated to support federated authentication. Also, the Node.js runtime that is used by the `devconsole` and `shell` utilities was updated to the latest `0.12.15` version.
* The buildpack adds support for the [Dynatrace Ruxit ![External link icon](../../icons/launch-glyph.svg "External link icon")](http://www.dynatrace.com/en/ruxit/) application monitoring agent.
* The buildpack provides an updated data collector for the [Monitoring and Analytics service](/docs/services/monana/index.html#monana_oview).
* The buildpack also provides an updated version of the agent for the [Auto-Scaling service](/docs/services/Auto-Scaling/index.html).
* The monthly Liberty runtime version was updated to the [2016.7.0.0](https://developer.ibm.com/wasdev/blog/2016/06/30/beta-websphere-liberty-and-tools-july-2016/) release.

### June 17, 2016: Updated Liberty buildpack v3.0-20160608-1450
* The buildpack now contains two versions of WebSphere Liberty, the latest stable release and the latest monthly release. Specifically, it provides [16.0.0.2](http://www-01.ibm.com/support/docview.wss?uid=swg21984970) stable release and [2016.6.0.0](https://developer.ibm.com/wasdev/blog/2016/06/03/beta-websphere-liberty-and-tools-june-2016/) monthly release. The stable release will be used by default. See [Liberty versions](buildpackDefaults.html#liberty_versions) for additional details.
* The buildpack also contains security fixes for the [Apache Standard Taglibs vulnerability](http://www-01.ibm.com/support/docview.wss?uid=swg21985531).

### May 25, 2016: Updated Liberty buildpack v2.9-20160519-1249
* The buildpack contains an updated version of WebSphere Liberty based on the [May beta](https://developer.ibm.com/wasdev/blog/2016/05/06/beta-websphere-liberty-and-tools-may-2016/). The updated version of Liberty makes the *bluemixLogCollector-1.1* and *logstashCollector-1.1* beta features available in {{site.data.keyword.Bluemix_notm}}.

### May 5, 2016: Updated Liberty buildpack v2.8-20160430-1011
* The buildpack contains an updated version of WebSphere Liberty based on the [April beta](https://developer.ibm.com/wasdev/blog/2016/04/08/beta-websphere-liberty-and-tools-april-2016/). The updated version of Liberty makes the *logstashCollector-1.0* GA feature and the *logmetCollector-1.0* beta feature available in {{site.data.keyword.Bluemix_notm}}.
* The buildpack also contains updated versions of IBM JRE: 8 SR3 and 7.1 SR3 FP40.
* The buildpack adds initial support for the [AppDynamics ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://www.appdynamics.com/) application monitoring agent.
* The [Dynatrace](dynatrace.html) support was improved to simplify the installation of the agent.
* The buildpack provides an updated data collector for the [Monitoring and Analytics service](/docs/services/monana/index.html#monana_oview). It contains a fix for a problem with collection of the max heap data.
* The Node.js runtime that is used by the [devconsole and shell App Management utilities](/docs/manageapps/app_mng.html#app_management) was updated to the latest 0.12.13 version.

### March 25, 2016: Updated Liberty buildpack v2.7-20160321-1358
* The buildpack contains an updated version of WebSphere Liberty based on the [March beta](https://developer.ibm.com/wasdev/blog/2016/03/18/new-websphere-liberty-features-march-2016/). The updated version of Liberty makes the cloudant-1.0 beta feature available in {{site.data.keyword.Bluemix_notm}}
* The buildpack also contains updated versions of IBM JRE: 8 SR2 FP12 and 7.1 SR3 FP32.
* The buildpack provides an updated version of the agent for the [Auto-Scaling service](/docs/services/Auto-Scaling/index.html).
* The buildpack now comes with a new data collector for the [Monitoring and Analytics service](/docs/services/monana/index.html#monana_oview). The new collector enables configuration of monitoring thresholds and contains a number of bug fixes.
* The buildpack provides an updated DB2® JDBC driver version 4.19.49.
* The Node.js runtime that is used by the [devconsole and shell App Management utilities](/docs/manageapps/app_mng.html#app_management) was updated to the latest 0.12.12 version.

### March 7, 2016: Updated Liberty buildpack v2.6-20160225-1649
* The buildpack adds support for Dynatrace application monitoring. See [Using Dynatrace](dynatrace.html) for details.
* The buildpack adds support for [DynamicPULSE](www.fujitsu.com/jp/group/fsweb/products/dynamic-pulse/).

### February 10, 2016: Updated Liberty buildpack v2.5-20160209-1336
* The buildpack contains an updated version of WebSphere Liberty based on the [February beta](https://developer.ibm.com/wasdev/blog/2016/02/12/beta-websphere-liberty-and-tools-february/). The updated version of the Liberty profile makes the apiDiscovery-1.0 GA feature available in {{site.data.keyword.Bluemix_notm}}.

### February 4, 2016: Updated Liberty buildpack v2.4-20160127-1437
* The buildpack contains an updated version of WebSphere Liberty based on the January beta. With this update, the scim-1.0 Liberty feature, previously available as beta a feature, is now available as a production-ready feature. The updated version of Liberty also makes the passwordUtilities-1.0 beta feature available in {{site.data.keyword.Bluemix_notm}}.
* The buildpack also contains an updated IBM JRE 7.1 SF3 FP20 and IBM JRE 8 SR2 FP10.
* The buildpack was updated to download the latest 1.x [MariaDB Connector/J JDBC driver ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://mariadb.com/kb/en/mariadb/about-mariadb-connector-j/) when performing [auto-configuration for MySQL type of services](autoConfig.html).

### December 16, 2015: Updated Liberty buildpack v2.3-20151208-1311
* The buildpack contains an updated version of the Liberty profile based on the [December beta](https://developer.ibm.com/wasdev/blog/2015/11/20/beta-was-liberty-beta-with-tools-december-2015/). The updated version of the Liberty profile makes the spnego-1.0 and wsSecuritySaml-1.1 GA features and the scim-1.0 beta feature available in {{site.data.keyword.Bluemix_notm}}.
* The buildpack also contains an updated IBM JRE 8 SR2.
* The buildpack was also updated to download the latest [9.4.x PostgreSQL JDBC driver ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://jdbc.postgresql.org/) and 1.2.x [MariaDB Connector/J JDBC driver ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://mariadb.com/kb/en/mariadb/about-mariadb-connector-j/) when performing [auto-configuration](autoConfig.html) for PostgreSQL or MySQL type of services.

### November 23, 2015: Updated Liberty buildpack v2.2-20151119-1720
* The buildpack contains an updated version of the Liberty profile runtime and WebSphere eXtreme Scale Client with security fixes for the [Apache Commons Collection vulnerability](http://www-01.ibm.com/support/docview.wss?uid=swg21971426).
* The buildpack also contains an updated version of the [Java MongoDB Driver ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://docs.mongodb.org/ecosystem/drivers/java/), v2.13.3. The new driver is compatible with MongoDB version 2.4, 2.6 and 3.0.
* The buildpack also provides an updated version of the data collector for the [Monitoring and Analytics service](/docs/services/monana/index.html). The updated data collector has improved method tracing capabilities.

### October 16, 2015: Updated Liberty buildpack v2.1-20151006-0912
* The buildpack contains an updated version of the Liberty profile based on the [October beta](https://developer.ibm.com/wasdev/blog/2015/09/25/beta-was-liberty-beta-with-tools-october-2015/). With this update, the bells-1.0, rtcomm-1.0, rtcommGateway-1.0, samlWeb-2.0, sipServlet-1.1 Liberty features, previously available as beta features, are now available as production-ready features.
* The buildpack also contains an updated IBM JRE 8 SR1 FP11.
* The buildpack also provides a number of performance improvements and optimizations:
  * The [CDI 1.2](optionsForPushing.html) implicit bean archive scanning feature is disabled by default when deploying WAR or EAR files.
  * To reduce the droplet size, the [App Management utilities](/docs/manageapps/app_mng.html) devconsole and shell, require a restage operation instead of a restart.
  * The IBM JRE's shared class cache is disabled as it was not being reused in the {{site.data.keyword.Bluemix_notm}} environment.

### September 18, 2015: Updated Liberty buildpack v2.0-20150914-1535
* The buildpack introduces two major changes:
  * The default configuration for WAR and EAR files enables Java EE 7 Web Profile features instead of Java EE 6 Web Profile features.
  * The default Java version is version 8 instead of version 7.
* Refer to the [Upcoming Liberty for Java buildpack changes](https://developer.ibm.com/bluemix/2015/09/08/upcoming-liberty-for-java-buildpack-changes/) blog post for details about these changes and how they may affect your application.
* The buildpack also introduces app_state configuration option to disable the appstate feature via the JBP_CONFIG_LIBERTY environment variable. The appstate feature integrates with the Cloud Foundry health check process to ensure the Liberty application is fully initialized before the application can receive HTTP requests. To disable the appstate feature, you can set the JBP_CONFIG_LIBERTY environment variable to “app_state: false”.

### September 4, 2015: Updated Liberty buildpack v1.22-20150824-1104
* The buildpack supports the [HTTP_PROXY and HTTPS_PROXY environment variables](environmentVariables.html). If set, the buildpack uses the proxy server specified by these environment variables when it downloads various buildpack components.

### August 19, 2015: Updated Liberty buildpack v1.21-20150811-1342
* The buildpack contains an updated version of the Liberty profile based on the [August beta](https://developer.ibm.com/wasdev/blog/2015/07/30/beta-was-liberty-beta-with-tools-august-2015/). The updated version of the Liberty profile makes the following new [beta features](usingBetaFeatures.html) available in {{site.data.keyword.Bluemix_notm}}: bells-1.0, rtcommGateway-1.0, samlWebSso-2.0.

### July 31, 2015: Updated Liberty buildpack v1.20.1-20150729-1255
* The buildpack contains updated versions of IBM JREs: 7.1 SR1 FP10 and 8 SR1 FP10.
The updated JREs contain [latest security fixes](http://www-01.ibm.com/support/docview.wss?uid=swg21964161) and other improvements.
* The service plug-in that provides [auto-configuration support](autoConfig.html) for the [Cloudant NoSQL Database](/docs/services/Cloudant/index.html#Cloudant) service was updated to ensure that the connections to the service are established over a secure channel.

### July 21, 2015: Updated Liberty buildpack v1.20-20150713-1450
* The buildpack contains an updated version of the Liberty profile based on the [8.5.5.6 release](https://developer.ibm.com/wasdev/blog/2015/06/25/java-ee-7-has-landed-in-was-liberty/). With this release all the Java EE 7 Liberty features previous available as beta features, are now available as production-ready features. Due to port and other restrictions in the {{site.data.keyword.Bluemix_notm}}, some features such as for example remote EJBs are not be fully supported in the platform.
* The buildpack recognizes and runs applications packaged in the [distZip-style ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://docs.gradle.org/current/userguide/application_plugin.html).
* The buildpack contains an updated data collector for the [Monitoring and Analytics Service](/docs/services/monana/index.html) and WebSphere eXtreme Scale Client that support the new Liberty runtime version.

### June 30, 2015: Updated Liberty buildpack v1.19.1-20150622-1509
* This version of the buildpack contains an updated IBM JRE with a security fix for the [LogJam vulnerability](http://www-01.ibm.com/support/docview.wss?uid=swg21961390).
* The [New Relic](newRelic.html) agent was updated to version 3.17. The new version provides improved integration with the Liberty profile runtime.

### June 14, 2015: Updated Liberty buildpack v1.19-20150608-1717
* The buildpack contains a number of application management enhancements that include support for the development console and web-based shell access. See the [app management documentation](/docs/manageapps/app_mng.html) for details.
* The buildpack also contains a fix for a problem where the Liberty feature for the [Monitoring and Analytics Service](/docs/services/monana/index.html) could not be found.

### May 27, 2015: Updated Liberty buildpack v1.18-20150519-1642
* The buildpack contains an updated version of the Liberty profile based on the [May beta](https://developer.ibm.com/wasdev/blog/2015/05/08/beta-liberty-and-tools-may-2015/).

### May 5, 2015: Updated Liberty buildpack v1.17-20150501-1729
* The buildpack contains an updated version of the Liberty profile based on the [April beta](https://developer.ibm.com/wasdev/blog/2015/04/10/announcing-liberty-beta-with-tools-aprilmay-2015/). With this update, the jsp-2.3, el-3.0, and jdbc-4.1 Liberty features, previously available as beta features, are now available as production-ready features. Also, additional Java EE 7 features such as jsf-2.2, javaMail-1.5, webProfile-7.0, and javaee-7.0 are now available as [beta features](usingBetaFeatures.html).
* The buildpack also provides initial support for Java 8. IBM JRE 7.1 remains the default JRE but IBM JRE 8 can be enabled for an application by setting the JBP_CONFIG_IBMJDK environment variable. Configuring version of OpenJDK is also supported. See [Customizing the JRE](customizingJRE.html) for all the details.
* The buildpack provides a new JBP_CONFIG_LIBERTY environment variable that can be used to override the default set of Liberty features enabled for an application when it deploys a WAR or EAR file. See [Stand-alone Applications](optionsForPushing.html#stand_alone_apps) for more information.
* The service plug-in for the [Monitoring and Analytics Service](/docs/services/monana/index.html) was updated to reduce the size of logs that are generated for the service.
* With this version of the buildpack, the way the application files are laid out in the droplet changed. The change in the file structure eliminated complexity that is related to maintaining symbolic links and should have no impact on the applications.

### April 15, 2015: Updated Liberty buildpack v1.16-20150407-1737
* This version of the buildpack contains an updated IBM JRE 7.1-2.11 with a [security fix for the Bar Mitzvah vulnerability](http://www-01.ibm.com/support/docview.wss?uid=swg21882777).
* When stand-alone WAR files are deployed, if provided, the buildpack now uses the context-root that is specified in the embedded **ibm-web-ext.xml** file as the application's context root. With this change, applications that were previously deployed under the root context might be deployed under a different context based on the settings in the **ibm-web-ext.xml** file.

### April 3, 2015: Updated Liberty buildpack v1.15-20150402-1422
* The buildpack contains an updated version of the Liberty profile based on the [March beta](https://developer.ibm.com/wasdev/blog/2015/03/13/announcing-liberty-beta-tools-march-2015/). The updated version of the Liberty profiles makes the jsf-2.2 beta feature available in {{site.data.keyword.Bluemix_notm}}.
* The buildpack also contains an updated version of the data collector for the [Monitoring and Analytics service](/docs/services/monana/index.html).

### March 20, 2015: Updated Liberty buildpack v1.14-20150319-1159
* This version of the buildpack contains an updated IBM JRE 7.1.2.11 with a security fix for the [FREAK vulnerability](http://www-01.ibm.com/support/docview.wss?uid=swg21699864).
* The [SQL Database](services/SQLDB/index.html#SQLDB) service offers paid plans that provide an option for connecting with the database server over the SSL protocol. The buildpack's auto-configuration support for SQL Database service was updated to configure the runtime to connect with the database over SSL if the SSL connection information is available.
* The buildpack was updated to report an error when a stand-alone WAR or EAR file that contains a **server.xml** configuration file in root of the application archive is deployed.
* The buildpack contains a fix for MongoDB's auto-configuration service plug-in that in certain cases generated an invalid **server.xml** configuration.

### February 10, 2015: Updated Liberty buildpack v1.13-20150209-1122
* The buildpack contains security fixes for the [Apache HttpComponents and Java overlay feature vulnerabilities](https://www-304.ibm.com/connections/blogs/PSIRT/entry/ibm_security_bulletin_multiple_vulnerabilities_fixed_in_liberty_for_java_for_ibm_bluemix_cve_2012_6153_cve_2014_3577_cve_2015_0178?lang=en_us).
* The buildpack contains an updated version of the Liberty profile based on the [February beta](https://developer.ibm.com/wasdev/blog/2015/02/13/announcing-liberty-beta-tools-february-2015/). The updated version of the Liberty profile provides an updated version of the WebSocket GA feature websocket-1.1. It also makes the following Java EE 7 beta features available in {{site.data.keyword.Bluemix_notm}}:
  * cdi-1.2, el-3.0, jsp-2.3, jca-1.7, jacc-1.5, and jaspic-1.1
* The buildpack provides integration with the [ZeroTrunaround's JRebel tool ![External link icon](../../icons/launch-glyph.svg "External link icon")](http://zeroturnaround.com/software/jrebel/). The integration makes it easy to use JRebel with {{site.data.keyword.Bluemix_notm}} applications and perform instant application updates without redeploying or restaging the application. Only stand-alone web applications are supported.

### February 6, 2015: Updated Liberty buildpack v1.12-20150130-1016
* The buildpack contains an updated version of the Liberty profile based on the [January beta](https://developer.ibm.com/wasdev/blog/2015/01/16/announcing-liberty-beta-tools-january-2015/).
* The buildpack contains a trimmed version of the data collector for the [Monitoring and Analytics service](/docs/services/monana/index.html#gettingstartedtemplate).

### January 23, 2015: Updated Liberty buildpack v1.11-20150119-1511
* The buildpack contains an updated IBM JRE version 7.1 SR2 FP1.
* It also contains an updated WebSphere eXterme Scale Client version 8.6.0.6 and updated agent for the Auto-Scaling service.
* The [New Relic](newRelic.html) service support was enhanced to support user-defined services.
* The buildpack was improved to report detailed versions of the Liberty profile and IBM JRE.

### December 19, 2014: Updated Liberty buildpack v1.10-20141218-0103
* The buildpack provides a development mode for applications. The development mode is a special mode that allows developers to conduct many activities for an application instance that were not possible before. By using this feature, this version of the {{site.data.keyword.eclipsetoolsfull}} can now support remote debugging with incremental file updates against a Liberty application that is running in {{site.data.keyword.Bluemix_notm}}. This makes it convenient for a developer that uses Eclipse to debug an application in the cloud and apply changes to that application instantly.
* The buildpack also contains an updated version of the Liberty profile based on the [December beta](https://developer.ibm.com/wasdev/blog/2014/12/10/announcing-liberty-beta-december/).
* In addition, the following four Liberty features that were previously available as beta features, are now production-ready:
  * concurrent-1.0
  * jsonp-1.0
  * servlet-3.1
  * websocket-1.0.
* The buildpack provides integration with the New Relic service. Once an application is bound to the New Relic service, the buildpack automatically downloads and configures the runtime with the New Relic agent.
* The buildpack has the following known limitations:
  * When in development mode, a SessionCache service cannot be bound.
  * When in development mode, a thread dump cannot be created.
  * When using the servlet-3.1 or websocket-v1.0 feature, the Monitoring & Analytics service cannot be bound.

### December 5, 2014: Updated Liberty buildpack v1.9-20141202-0947
* The buildpack provides an enhanced JVM option support. The JVM options can now be applied with a restart operation. Restaging of the application is not necessary. Also, the default JVM options are optimized for fast failure and pre-configured with a common location that makes it easy to find the generated dumps. More details are provided in the [Custom Configuration of Java JVM for the Liberty Runtime article](https://developer.ibm.com/bluemix/2014/12/12/custom-configurations-java-jvm-liberty-runtime/).
* The buildpack contains an updated DB2 JDBC driver version 4.17.29.
* It also contains a fix for a problem that prevented collection of the Liberty thread pool usage information for the Monitoring & Analytics service.

### November 21, 2014: Updated Liberty buildpack v1.8-20141118-1610
* The buildpack contains an updated IBM JRE version 7.1 SR2 that provides a fix for the [POODLE vulnerability](http://www-01.ibm.com/support/docview.wss?uid=swg21687173).
* It also contains an updated version of the Liberty profile based on the [November beta](https://developer.ibm.com/wasdev/blog/2014/11/07/announcing-liberty-profile-beta-november/).

### October 30, 2014: Updated Liberty buildpack v1.7-20141020-1759
* The buildpack contains an updated IBM JRE version 7.1 SR1 FP3.
* It also provides a fix for a problem that prevented deployment of applications with server configuration that contained Unicode characters.

### October 23, 2014: Updated the Liberty Buildpack v1.6-20141013-1628
* The buildpack now comes with a new data collector for the [Monitoring and Analytics](/docs/services/monana/index.html). The new data collector collects diagnostic deep dive information, which enables users of the Diagnostics plan of the service to diagnose problems with their applications, down to the specific line of code.
* The buildpack contains updated versions of the management and auto-scaling agents that include bug fixes and minor improvements. It also includes an updated version of the [Liberty profile](https://developer.ibm.com/wasdev/) and [Java MongoDB Driver ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://docs.mongodb.org/ecosystem/drivers/java/), v2.12.3.
* In the cloudAutowiring feature, a bug that caused resource injection errors in some applications was fixed.

### October 3, 2014: Updated Liberty Buildpack v1.5-20140923-1143
* With the updated buildpack, the applications can now use the Liberty beta features, including WebSocket 1.0, Servlet 3.1, or JAX-RS 2.0. For more information, see [Using the beta features](usingBetaFeatures.html).

### September 30, 2014: Updated Liberty Buildpack v1.4-20140908-1803
* The buildpack now provides support for ElephantSQL and ClearDB MySQL Database third-party services. The auto-configuration support also works with posgresql and mysql experimental services. With the new total of 13 services, the auto-configuration support in the Liberty buildpack makes it quicker and easier to consume {{site.data.keyword.Bluemix_notm}} services in Liberty applications.
* During application staging the buildpack displays improved log messages about auto-configuration and other actions it takes.
* The buildpack contains an updated version of Liberty profile with fixes and improvements.
* It also contains an updated version of IBM JRE version 7.1 that has performance improvements. See the [What's new](http://www-01.ibm.com/support/knowledgecenter/SSYKE2_7.0.0/com.ibm.java.lnx.71.doc/diag/preface/changes_71/changes.html) page for detailed set of changes.

### August 28, 2014: Updated Liberty Buildpack v1.3-20140818-1538
* The buildpack contains an updated version of the [Liberty Profile](https://developer.ibm.com/wasdev/) with the latest fixes and improvements.
* This version of the buildpack fixes support for the JAVA_OPTS environment variable for passing additional JVM options to the application runtime.
* It also fixes a problem that prevented deployment of standalone Spring-based Jar applications.
* It is now possible to generate and download IBM JVM snap traces using the {{site.data.keyword.Bluemix_notm}} UI. See the [Troubleshooting topic](http://www-01.ibm.com/support/knowledgecenter/SSYKE2_7.0.0/com.ibm.java.lnx.70.doc/troubleshooting.html) in the IBM JVM documentation to learn more about the snap traces or other diagnostic information that is generated by the JVM.

### July 29, 2014: Updated Liberty Buildpack v1.1-20140725-1341
* The new version of Liberty’s {{site.data.keyword.Bluemix_notm}} Edition is here!
  * With this version of Liberty, there are fixes in addition to new features that allow you to consume {{site.data.keyword.Bluemix_notm}} services more effectively!
  * With the new CouchDB feature available, the Cloudant® service can now automatically configure it so that a connector object is handily available! Parsing through VCAP_SERVICES and providing the ektorp client jars is no longer necessary.
* The new version of IBM SDK for Java is here!
  * When your applications are pushed again, they use IBM SDK for Java Version 7.1-1.0. This comes with a substantial performance upgrade. Your application shows better throughput and reduced memory usage. See more about the IBM Java SDK [here](http://www-01.ibm.com/support/docview.wss?uid=swg21671466).

# rellinks
{: #rellinks notoc}
## general
{: #general notoc}
  * [Liberty runtime](index.html)
  * [Liberty Profile Overview](http://www-01.ibm.com/support/knowledgecenter/SSAW57_8.5.5/com.ibm.websphere.wlp.nd.doc/ae/cwlp_about.html)
