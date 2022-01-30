# Elliptic Curve Encryption
This is my implementation of an Elliptic Curve Encryption System using the Python Library PyFinite. 
## Results: 
encryption(24) &#8594; [1155779365684273444227653099536, 653610295036787900097192168556, 218439540478955744436474849301, 357140456979494963198197555111, 249, 453511634163535756719750784985]

decryption([1155779365684273444227653099536, 653610295036787900097192168556], [218439540478955744436474849301, 357140456979494963198197555111], 249, 453511634163535756719750784985) &#8594; [24, 31]

## Project Overview: 
![image](https://user-images.githubusercontent.com/79173446/151675339-ff511028-00f2-47b7-b66e-4c86083d2d54.png)

Elliptic Curve Encryption uses Finite Field Theory to encrypt numbers. In contrast to normal Elliptic Curves over a standard Cartesian Plane, Elliptic Curves over Finite Fields look like the one above, and the traditional operatiosn of addition, subtraction, multiplication, and division are replaced with their counterparts on the Finite Field. 

The Encrpytion happens via two methods, Scalar_Add and Scalar_Multiplication. Thinking about Scalar_Add, imagine we have two points on the curve above, a and b. if we draw a line in between these two points and continue the line so that when it hits one of the edges, it goes to the other side, we will eventually get another point. This new point reflected over the middle is the sum of these two points. Scalar_Multiplication is simply this process repeated over and over again. The program encrypts by performing Scalar_Multiplication on a point many times. 
