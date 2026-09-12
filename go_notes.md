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