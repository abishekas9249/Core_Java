### Servlet in Java by Extending to a Source Class Java File

```java
package org.virtusa;

import java.io.IOException;
import java.io.PrintWriter;

import javax.servlet.Servlet;
import javax.servlet.ServletConfig;
import javax.servlet.ServletException;
import javax.servlet.ServletRequest;
import javax.servlet.ServletResponse;

public class HelloServlet implements Servlet {

	@Override
	public void destroy() {
		// TODO Auto-generated method stub
		
	}

	@Override
	public ServletConfig getServletConfig() {
		// TODO Auto-generated method stub
		return null;
	}

	@Override
	public String getServletInfo() {
		// TODO Auto-generated method stub
		return "Hello World Info";
	}

	@Override
	public void init(ServletConfig serve) throws ServletException {
		System.out.println("Servlet Initialized");
		
	}

	@Override
	public void service(ServletRequest req, ServletResponse res) throws ServletException, IOException {
		System.out.println("Service  Called");
		PrintWriter pw=res.getWriter();
		pw.println("<html>");
		pw.println("<body>");
		pw.println("<h1>Hello World<h1>");
		pw.println("</body>");
		pw.println("</html>");
	}

}
```

## Creating web.xml file to run using tomcat server version 9.0
```xml
<?xml version="1.0" encoding="UTF-8"?>
<web-app xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns="http://xmlns.jcp.org/xml/ns/javaee" xsi:schemaLocation="http://xmlns.jcp.org/xml/ns/javaee http://xmlns.jcp.org/xml/ns/javaee/web-app_4_0.xsd" id="WebApp_ID" version="4.0">
  <display-name>ServletDemo</display-name>
  <servlet>
  	<servlet-name>Hello</servlet-name>
  	<servlet-class>org.virtusa.HelloServlet</servlet-class>
  </servlet>
  <servlet-mapping>
  	<servlet-name>Hello</servlet-name>
  	<url-pattern>/hello</url-pattern>
  </servlet-mapping>
</web-app>
```
