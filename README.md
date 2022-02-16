# Assemby-Inverse-Matrix
부동소수점으로 이루어진 N*N(1<=N<=20)정방행렬에 대한 역행렬을 가우스 소거법을 통하여 구하는 프로그램

## Language
  * Assembly
## 부동소수점 곱셈(radix-4) Flow chart
  * multiplicand=A
  * multiplier=X
  * Overflow=V
  * Result=U
<img  width="300" alt="Multiple_flow_chart" src="https://user-images.githubusercontent.com/56907015/154195593-ee32e9bd-2648-40bc-9930-6d722800f4d4.png">

## 부동소수점 나눗셈 Flow chart
<img height="700" alt="division_flow_chart" src="https://user-images.githubusercontent.com/56907015/154195767-2833c8d3-d3a8-4f7a-a54b-878ea36ceb29.png">

## 역행렬 의사코드
{Matrix | inverse matrix}순으로 a[n][n*2]이라고 하면
```
for (i=0 to n) 
 t=a[i][i]
 if(t==0)
    find t
 exchange line
 for( j=i to n*2)
    a[i][j]=a[i][j]/t
 for(l=0 to n)
    if(i!=l)
        h=a[l][i]
 for(k=0 to 2*n)
    a[l][k]=a[l][k]-h*a[i][k]
```
## Input Data 예제
<img height="200" alt="division_flow_chart" src="https://user-images.githubusercontent.com/56907015/154198750-b59d5359-4b50-48f5-87a0-470bfa123281.png">

## Reference 
* D. M. Harris and S. L. Harris, Digital design and computer architecture, Morgan Kaufmann, 2007
