# The Idea Behind Big O Notation

Big O notation is the language we use for talking about how long an algorithm takes to run.

With Big O notation, we express the runtime in terms of how quickly it grows relative to the input.

1. How quickly the runtime grows - It's hard to pin down the exact runtime of an algorithm. It depends on the speed of the processor, what else the computer is running, etc. So instead of talking about the runtime directly, we use big O notation to talk about how quickly the runtime grows.

2.  Relative to the input - If we were measuring our runtime directly, we could express our speed in seconds. Since we're measuring how quickly our runtime grows, we need to express out speed in terms of... something else. With big O notation, we use the size of the input, which is usually called $n$. This is so we can express it as $O(n)$.

## Examples
```c++
void printFirst(){
	cout << arr[0];
}
```