# auth-server


To generate key-pair use the below command.

```
keytool -genkeypair -alias mytest -keyalg RSA -keypass mypass -keystore mytest.jks -storepass mypass
```


To get the public key.
 
```
keytool -list -rfc --keystore mytest.jks | openssl x509 -inform pem -pubkey
```

##References
[Spring-security OAuth JWT tutorial on Baeldung](http://www.baeldung.com/spring-security-oauth-jwt)  
[JWT OAuth tutorial on Spring Guides](https://github.com/spring-guides/tut-spring-security-and-angular-js/blob/master/oauth2/authserver/src/main/java/demo/AuthserverApplication.java)