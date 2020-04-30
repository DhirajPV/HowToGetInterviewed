# ⭕ Big O (my god this is exciting)

## Things to remember and notes:
### Big O:

$$f(n) \in O(g(n)) \longleftrightarrow \exists c \in \mathbb{R}_{>0},n_0 \in \mathbb{N},\forall n \in \mathbb{N}, n\geq n_0 \implies f(n) \leq c\cdot g(n)$$

### **Big Omega:**

$$f(n) \in \Omega(g(n)) \longleftrightarrow \exists c \in \mathbb{R}_{>0},n_0 \in \mathbb{N},\forall n \in \mathbb{N}, n\geq n_0 \implies f(n) \ge c\cdot g(n)$$

### **Big Theta**

$$f(n) \in \Theta(g(n)) \iff f(n) \in O(g(n)) \land f(n) \in \Omega(g(n))$$

### Little o and little omega

$$f(n) \in o(g(n)) \longleftrightarrow \forall \epsilon \in \mathbb{R}_{>0}, \exists n_0 \in \mathbb{N},\forall n \in \mathbb{N}, n\geq n_0 \rightarrow f(n) < \epsilon\cdot g(n)$$

$$f(n) \in \omega(g(n)) \longleftrightarrow \forall \epsilon \in \mathbb{R}_{>0}, \exists n_0 \in \mathbb{N},\forall n \in \mathbb{N}, n\geq n_0 \rightarrow f(n) > \epsilon \cdot g(n)$$

The following definitions using limits are equivalent:

$$f(n) \in o(g(n)) \longleftrightarrow \lim_{n\rightarrow \infty} \frac{f(n)}{g(n)} = 0$$

$$f(n) \in \omega(g(n)) \longleftrightarrow \lim_{n\rightarrow \infty} \frac{f(n)}{g(n)} = \infty$$



### Runtimes you need to memorize
* Insertion Sort, Selection Sort and Quicksort: O(n<sup>2</sup>)
* Mergesort, Heapsort: O(n log n)
*


## Questions: 
1)
~~~
int product(int a, int b){
    int sum = 0; 
    for(int i = 0; i < b; i++){
        sum +=a;
    }
    return sum; 
}
~~~

2)
~~~
int power(int a, int b) { 
    if (b < 0) {
        return 0;
    }
        
    else if (b == 0) {
        return 1;
    }
    
    else {
        return a * pow(a, b - 1);
    }
~~~

3)
~~~
int sqrt(int x){
    for (int i = 0; i < x; i++){
        if (pow(i, 2) == x){
            return i; 
        }
    }
}
~~~
4) 
~~~
int intersect(int[] a, int[] b){
    mergesort(b);
    int intersect = 0; 
    
    for (int x : a) {
        if (binarySearch(b, x) >= 0) {
            intersect++;
        }
    }
    return intersect; 
}
~~~

5) 
~~~
~~~


