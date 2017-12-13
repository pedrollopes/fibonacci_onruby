# fibonacci_onruby

Recently I found myself in some trouble doing a test, where I had to elaborate the fibonacci sequence.
Them I asked some people, and they also had some trouble, so I researched and I will share what I got.

I hope this helps you.


## X number from Fibonnaci sequence.

So, this will give you the number X from the fibonacci sequence

```
def fibonacci( n )
    return  n  if n <= 1 
    fibonacci( n - 1 ) + fibonacci( n - 2 )
end 
puts fibonacci( 10 )
# => 55
```

Same result but One Liner:

```
def fibonacci(n)
   n <= 1 ? n :  fibonacci( n - 1 ) + fibonacci( n - 2 ) 
end
puts fibonacci( 10 )
# => 55
```

## If you need a function which returns the nth number in Fibonacci sequences with an input n, this may help you:

```
def fib(n)
  n <= 2 ? 1 : fib(n - 1) + fib(n - 2)
end

a = gets.to_i
p (1..a).map {|i| fib(i)}
```

a = 10 may give you the following result:

```# => [1, 1, 2, 3, 5, 8, 13, 21, 34, 55]```

