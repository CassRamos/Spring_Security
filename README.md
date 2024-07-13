<h1 align="center"> Spring Security </h1>
<p align="center">
  <a href="#-tecnologies">Tecnologies</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-project">Project</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#memo-license">License</a>
  <p align="center">
  <img alt="License" src="https://img.shields.io/static/v1?label=license&message=MIT&color=49AA26&labelColor=000000">
</p>
</p>
<p align="center">
This repository is a back-end file of server_app application<br/>
</p>

<br>
<br>

## 🚀 Tecnologies

This project was developed with the following technologies:

- Java & Spring Boot
- JWT
- PostgreSQL
- Postman 
- Git & Github 

 <br>

## 💻 Project

This project contributes to the application and understanding of the use of tokens, utilizing JWT. Additionally, other features such as logout, refresh token, and password change have been added.

<br>

## :memo: License


This project is under license from MIT

<br>

## Endpoints 
<p>To test the application endpoints you can use the Postman, HttpPie, Insomnia...</p>

<br>

### Register user
 - <p> To register a user, you'll use: </p>
<p align="center">
  <img alt="User register" src="./img/register.png" width="80%">
</p>

<br>

### Auth user
 - <p> After registering the user, it's necessary to input the "access_token" value, along the email and password, in the body of the request. In this way, a new access token will be generated: </p>
<p align="center">
  <img alt="User auth" src="./img/auth.png" width="80%">
</p>

<br>

### Access 
 - <p> To access a secured endpoint, input the new access token generated at the "\auth" endpoint:</p>
<p align="center">
  <img alt="Access secured" src="./img/access.png" width="80%">
</p>

<br>

### Refresh token
 - <p> To generate a refresh token, it's necessary to input the current token. In this way, you will receive a new access token, and the previous token (which was used to generate this new token) will be invalidated: </p>
<p align="center">
  <img alt="Refresh token" src="./img/refresh.png" width="80%">
</p>

<br>

 - <p> Using this new access token, this should be the received response: </p>
<p align="center">
  <img alt="Access after refresh token" src="./img/access_ok_refresh.png" width="80%">
</p>

<br>

 - <p> Tryng to use the previous token, this is the response: </p>
<p align="center">
  <img alt="Access revoked after refresh token" src="./img/access_revoked_after_refresh.png" width="80%">
</p>

<br>

### Logout
 - <p> To perform logout, simply input the current access token: </p>
<p align="center">
  <img alt="Logout" src="./img/logout.png" width="80%">
</p>

<br>

 - <p> Tryng to use the invalidated token, this is the response: </p>
<p align="center">
  <img alt="Access revoked after logout" src="./img/access_revoked_after_logout.png" width="80%">
</p>

<br>

<p>Thanks for your attention, see you next time 💜</p>

