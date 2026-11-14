input

recursive formula: a(n) = a(n-1) + a(n-2) = ....

nthFibonacci(int n){       
        // Base case
        if (n <= 1) {
            return n;
        }
        
        // Recursive case
        return nthFibonacci(n - 1) + nthFibonacci(n - 2);
    }

while (length >= 0):
    FIBO.append(nthFibonacci(length))
    length -= 1
    
n = mem[INPUT]
offset, a, b = 0, 0, 1
if n <= 0: halt()
while True:
    mem[FIBO + offset] = a
    a, b = b, a + b
    offset += 4
    n -= 1
    if n != 0: continue
    break
halt()

