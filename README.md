第一轮考核
P1046
package main

import  "fmt"  

func main() {

	var s1 = make([]int, 10, 10)

	var x int

	var flag int

	cnt:=0

	for i := 0; i < 10; i++ {

		fmt.Scan(&x)

		s1[i] =x

}

  

	fmt.Scan(&flag)

	for i := 0; i < 10; i++ {
	
	if s1[i]<=flag+30 {

	cnt++
	
	}

}

	fmt.Println(cnt)

}
P1001
package main

import  "fmt"

func main() {
	var a int
	var b int
	
	fmt.Scan(&a)
	fmt.Scan(&b)

	fmt.Println(a+b)
}
P5737
package main

  

import  "fmt"

  

func main() {

	var a int

	var b int

	fmt.Scan(&a)
	fmt.Scan(&b)	
	
	s1 := make([]int,1500,1500)

	cnt:=0

	for i := a; i <= b; i++ {

		if (i%400 == 0) || (i%100 != 0 && i%4 == 0) {

		s1[cnt]=i

		cnt++

	}

}

	fmt.Println(cnt)

	for i:=0;i<cnt;i++{

	fmt.Printf("%d ",s1[i])
	
	}

}
PAtCoder ARC017A
package main

import  "fmt"

	func isPrime(x int)bool {
	
		if x <= 1 {

			return  false

}
  
for i:=2; i*i<=x; i++{

	if x%i == 0{

	return  false

	}
}

	return  true

}

  

func main(){

	var x int

	fmt.Scan(&x)

	if isPrime(x)==true {

		fmt.Println("YES")

}else {

	fmt.Println("NO")

	}

}
Bonus
1.九九乘法表
package main

import  "fmt"

func main() {

//for循环
for i := 1; i <= 9; i++ {
	for j := 1; j <= i; j++ {
	
	fmt.Printf("%d * %d = %d\t",j,i,i*j)
	
}

	fmt.Println()

	}

}
