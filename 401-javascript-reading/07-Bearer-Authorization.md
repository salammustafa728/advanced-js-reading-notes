# Bearer Authorization

## 1. **JWTs Explained**

JWT stands for: JSON Web Token and it's open standard, used to securely transfer information between bodies. also the info trusted and verified.
and it compact and self contained.

JWT useful for:
1. Authintecation
2. Information exchange

![jwt](https://www.vaadata.com/blog/wp-content/uploads/2016/12/JWT_tokens_EN.png)

## 2. **Intro to JWT**

JSON Web Token structure it's compact form consist of three parts separated by dots are 
1. Header: consists of two parts: the type of the token and the signing algorithm being used
2. Payload: contains the claims. There are three types of claims: registered, public, and private claims.
3. Signature: you have to take the encoded header, the encoded payload, a secret, the algorithm specified in the header, and sign that.

and it look like: 
>xxxxx.yyyyy.zzzzz

![jwt](https://miro.medium.com/max/1200/1*u3a-5xZDeudKrFGcxHzLew.png)



## 3. Are JWTs Secure?

Yes, it's because if you did any changes you won't be able to reach the data. no one can know the secret. JWT doesn't concern itself with encryption. It cares about validation. 

### npm jsonwebtoken docs

if you want to use the jwt you should install it 

>$ npm install jsonwebtoken

and we can use it in many different way with different method like decode incode or verfiy...etc. 

[Home](README.md)