# LU-Decomposition-for-Upper-Hessenberg-Matrix
### Introduction to LU decomposition
LU decomposition of a matrix is the factorization of a given square matrix into two triangular matrices, one upper triangular matrix and one lower triangular matrix, such that the product of these two matrices gives the original matrix. This method of factorizing a matrix as a product of two triangular matrices has various applications such as a solution of a system of equations, which itself is an integral part of many applications such as finding current in a circuit and solution of discrete dynamical system problems; finding the inverse of a matrix and finding the determinant of the matrix. 

A square matrix A can be decomposed into two square matrices L and U such that A = L U where U is an upper triangular matrix formed as a result of applying the Gauss Elimination Method on A, and L is a lower triangular matrix with diagonal elements being equal to 1.

![image](https://user-images.githubusercontent.com/125180530/219429450-0703379b-2866-4a6c-9d57-78195192bf0a.png)

![image](https://user-images.githubusercontent.com/125180530/219429590-9ed7ae1e-9d91-4a40-bbdd-589eb764ee13.png)

### LU decomposition for Upper Hessenberg Matrix
The difference between the general LU decomposition and this case is in the form of the input matrix. In the general case, we may have a matrix that its elements which are below the diagonal elements are non-zero however, in the Upper Hessenberg matrix the elements below the diagonal ones, except one element, are all zero. So, if we want to follow the process of LU decomposition for the Upper Hessenberg matrix, we have to do more operations although there is no need to do so. So, we change the process to reduce the number of operations and also the time that needs to be spent finishing the algorithm. 

### Concept or Flop
Complexity can be expressed in terms of floating point operations or flops required to find the solution, expressed as a function of the problem dimension. A Flop serves as a basic unit of computation. It could denote an addition, subtraction, multiplication, or division of two floating point numbers. In practice, a division is more expensive to compute. However, we approximate it to one flop to simplify the overall calculation. In this way, the number of flops indicates the cost of performing a sequence of operations. Note that, the flop count is just a rough measure of how expensive an algorithm can be. 

There are different kinds of flops:

![image](https://user-images.githubusercontent.com/125180530/219454156-d1ed325e-5b1c-402f-94f9-c8160edcd123.png)

![image](https://user-images.githubusercontent.com/125180530/219454210-072f38e0-7328-4b7c-82b3-a2ed694b3357.png)

![image](https://user-images.githubusercontent.com/125180530/219454282-4365cf2c-c5b8-4ac7-9c7a-65cd6129581b.png)

### Conclusion
With the use of the flop concept, we can come to the conclusion that for matrices in general the number of flops is greater than when we have the Upper Hessenberg matrix. So, for faster calculation and to avoid wasting time and doing useless operations, we write another function for LU decomposition of the Upper Hessenberg matrix. 
