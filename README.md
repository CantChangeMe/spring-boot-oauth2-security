# spring-boot-oauth2-security
This repository implements oauth2 security using  github in spring-boot.

Steps to secure your APIs using OAUTH2:

1.Add these dependencies:
<pre>
spring-boot-starter-web
spring-cloud-starter-securit
spring-cloud-starter-oauth2
</pre>
2.Annotate your springboot entry class with @EnableOAuth2Sso

3.Create Oauth2 application in gitgub to get client-id and client-secret.

4.Create application.yml file.
with below information:
<pre>
security:
  oauth2:
    client:
      client-id:
      client-secret:
      access-token-uri:
      user-authorization-uri:
      client-authentication-scheme:
    resource:
      user-info-uri:
      prefer-token-info:
</pre>

You are done.Now access APIs, they will ask github credentials to access them.
      
      
    



