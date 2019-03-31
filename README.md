# REST_jars
This contains all the jars required to build REST web service
Need to add this configuration in web.xml

<servlet>
  	<servlet-name>AnyName</servlet-name>
  	<servlet-class>org.glassfish.jersey.servlet.ServletContainer</servlet-class>
  	<init-param>
  		<param-name>jersey.config.server.provider.packages</param-name>
  		<param-value>Your service class package name</param-value>
  	</init-param>
  	<load-on-startup>1</load-on-startup>
  </servlet>
  <servlet-mapping>
  	<servlet-name>The name give to servlet tag above(AnyName)</servlet-name>
  	<url-pattern>/vikas/*</url-pattern>
  </servlet-mapping>
