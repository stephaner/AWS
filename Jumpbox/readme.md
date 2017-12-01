
# Set up of a Jumpbox on AWS Linux
## Create a VPC
![1](https://user-images.githubusercontent.com/33963568/33501890-391e57c6-d6ac-11e7-97e8-0364e4b9dee0.png)

## Create Subnets
![2](https://user-images.githubusercontent.com/33963568/33501891-39458792-d6ac-11e7-95f3-0afa73fb64dc.png)
![3](https://user-images.githubusercontent.com/33963568/33501892-3965073e-d6ac-11e7-86e6-98d542f53dc6.png)

## Create Route Tables
![4](https://user-images.githubusercontent.com/33963568/33501893-3982cc10-d6ac-11e7-9714-0e4f87b27e17.png)
![5](https://user-images.githubusercontent.com/33963568/33501894-39a01284-d6ac-11e7-9c48-aa1d08ddfc9b.png)

## Associate subnets to Route Tables
![6](https://user-images.githubusercontent.com/33963568/33501895-39bd626c-d6ac-11e7-83ed-52a2c1c254d1.png)
![7](https://user-images.githubusercontent.com/33963568/33501896-39d88d58-d6ac-11e7-8c92-bdac83bac329.png)

## Create Internet Gateway
![8](https://user-images.githubusercontent.com/33963568/33501897-39fb451e-d6ac-11e7-8775-c848f35f9fc2.png)

## Attach it to VPC
![9](https://user-images.githubusercontent.com/33963568/33501898-3a1e1c06-d6ac-11e7-8f25-91b6ee3de332.png)

## Add internet Gateway to Public Route Table
![10](https://user-images.githubusercontent.com/33963568/33501899-3a4844c2-d6ac-11e7-931a-2f3266ebdf78.png)

## Create Security Group for EC2 instances
![11](https://user-images.githubusercontent.com/33963568/33501900-3a67a07e-d6ac-11e7-9890-d8382b4ab9d0.png)

## Create Instance in public subnet
![12](https://user-images.githubusercontent.com/33963568/33501903-3a8711de-d6ac-11e7-88fb-373837d68e0e.png)
![13](https://user-images.githubusercontent.com/33963568/33501904-3ab3f410-d6ac-11e7-8f65-6cb139f68e66.png)

## Create Instance in private subnet
![14](https://user-images.githubusercontent.com/33963568/33501905-3ad1aba4-d6ac-11e7-9793-30172ef88d2e.png)

## Transfer private key to instance in public subnet

![15](https://user-images.githubusercontent.com/33963568/33501906-3b01ffac-d6ac-11e7-8cdd-c53728caa6b7.png)

## Connection to instance in private subnet
![16](https://user-images.githubusercontent.com/33963568/33501908-3b262f08-d6ac-11e7-8d85-f9ca1baedf1f.png)

## Connection to instance in public subnet
![17](https://user-images.githubusercontent.com/33963568/33501909-3b455978-d6ac-11e7-8dca-0337c024b677.png)
