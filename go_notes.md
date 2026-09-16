x := 1
x = "i" // error: '"i"' (type string) cannot be represented by the type int

data types:
boolean
int, int8, int16, int32, int64
uint, uint8, uint16, uint32, uint64, uintptr
float32, float64
complex64, complex128
byte
rune

var x int = 6
var y = 5 // works

const a = 5
a = 4 // error: Cannot assign to a

const b int = 5
const c = 4 // works

var x []int
x[0] = 1 // error: index out of range [0] with length 0

z := []int{1, 2, 3, 4, 5, 6, 7}
t1 := z[1:]  // [2 3 4 5 6 7]
t2 := z[:4]  // [1 2 3 4]
t3 := z[2:5] // [3 4 5]

s := "Hello"
s[0] = "X" // error: Cannot assign to s[0]

var f float32 = 0.123456789 // 0.12345679

f := 5.0
i := 1
r := f / i // error: f / i (mismatched types float64 and int)

func(a, b int)

type Rectangle struct {
	width, height float64
}

convention: error messages should be lowercase

type error interface {
	Error() string
}

note: defer -> lifo

x := 10
defer fmt.Println("x:", x)
x = 20
fmt.Println("x:", x)
// x: 20
// x: 10

for i := range 3 { ... } // 0, 1, 2

s := make([]int, 2)
s[0], s[1] = 1, 2

func sum(a, b int) (result int) {
	result = a + b
	return
}

var x any = "Hello"
t := x.(int)
fmt.Println(t) // panic: interface conversion: interface {} is string, not int

r, ok := x.(int)

s1 := make([]int, 2)
fmt.Println(s1) // [0 0]

var s2 []int
fmt.Println(s2) // []

s := make([]int, 2, 4)
s = append(s, 1, 2, 3, 4, 5, 6)
fmt.Println("len:", len(s)) // 6
fmt.Println("cap:", cap(s)) // 8 (if len > cap, cap will increase)