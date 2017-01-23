## Weblogic 12.2.1 Rest with Jaxrs 2.5.1 Hello World

This is simple rest using jersey. I had an error with the mapping in the web.xml

So i post this the fix to use the servlet-mapping.

I used the example from mkyong in this url:

<https://www.mkyong.com/webservices/jax-rs/jersey-hello-world-example/>


```xml
<servlet>
        <servlet-name>javax.ws.rs.core.Application</servlet-name>
    </servlet>

    <servlet-mapping>
        <servlet-name>javax.ws.rs.core.Application</servlet-name>
        <url-pattern>/rest/*</url-pattern>
    </servlet-mapping>
    ```