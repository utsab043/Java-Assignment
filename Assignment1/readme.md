# Anonymous Arrays In Java

An array without any name is called an anonymous array. Features of an anonymous array are:

* It has no name (obviously).
* It is created using the new keyword and pair of curly braces.
* It is created and initialized at the same time.
* It can be passed as an argument to a method.
* It can be of any dimension. e.g Two-dimensional (discussed later).

### 1. Syntax
Syntax to declare a one-dimensional anonymous array is :

new type[]{data_separated_by_comma}

// Example 1 : An anonymous array of first 4 primes.
new int[]{2, 3, 5, 7};
// Example 2 : An anonymous array of some fruit names.
new String[]{"Orange", "Apple", "Mango", "Banana", "Peach"];

### 2. It is created an initialized at the same time
All anonymous arrays of any data type are created and initialized at the same time using the new keyword and pair of curly braces.

Example:
```javascript
public class Anonymous_Demo_1 {
    public static void main(String[] args){
        // Method Arrays.toString takes and array and converts it into string.
        // An anonymous array of type int is being passed as an argument.
        System.out.println(Arrays.toString( new int[]{2, 3, 5, 7} ));
        // An anonymous array of type String is being passed as an argument.
        System.out.println(Arrays.toString(
                new String[]{"Orange", "Apple", "Mango", "Banana", "Peach"}));
    }
}
```
Output :
[2, 3, 5, 7]
[Orange, Apple, Mango, Banana, Peach]
 
### 3. It can be passed as an argument to a method
Anonymous arrays are often used along with methods. When an array is needed only to pass a collection of data to a method and not needed afterwards, an anonymous array is made. Like one in the last example. Let’s have another example:

Example:
```javascript
public class Anonymous_array_and_methods {
    // This method returns the sum of all elements of an array.
    public static int getSum(int[] Arr){
        int sum=0;
        for(int i=0 ; i<Arr.length ; ++i){
            sum = sum + Arr[i];
        }
        return sum;
    }

    public static void main(String[] args){
        // Passing an anonymous array to the method.
        int total = getSum(new int[]{2, 3, 5, 7, 11, 13});
        System.out.println("Array sum = " + total);
    }
}
```
Output :
Array sum = 41
 
### 4. Two dimensional anonymous array
We can have an anonymous array of any dimension. To declare an anonymous array of N dimensions, you need to put N pair of brackets after the data type and accordingly use the curly braces.

// An anonymous array in 2 dimension.
new int[][] {{1, 2, 3}, {1, 2}, {1, 2, 3, 4, 5}};

// An anonymous array in 3 dimension.
new int[][][]{
    {{1, 2, 3}, {1, 2}, {1, 2, 3, 4, 5}},
    {{9}, {9, 8, 7}, {9, 8, 7, 6, 5, 4}}
}

Example:
```javascript
public class twoD_Demo {
    // It takes two dimensional integer array and returns sum of its elements.
    public static int getSum(int[][] Arr){
        int sum=0;
        for(int i=0 ; i<Arr.length ; ++i){
            for(int j=0 ; j<Arr[i].length ; ++j){
                sum = sum + Arr[i][j];
            }
        }
        return sum;
    }
    public static void main(String[] args){
        int total = getSum(new int[][] {{1, 2, 3}, {1, 2}, {1, 2, 3, 4, 5}});
        System.out.println("Array sum = " + total);
    }
}
```
Output:
Array sum = 24
 
### 5. An anonymous array can be given a name as well.
If we want, we can give a name to an anonymous array. But after that it will no longer be anonymous.
Example:
```javascript
public class Naming_Demo {
    public static void main(String[] args){
        /*  An anonymous array is created and assigned to the
            array variable primes.
         */
        int[] primes = new int[]{2, 3, 5, 7, 11, 13, 17, 19, 23};
        /*  That array is no longer anonymous because it can be
            referenced using name primes.
         */
        System.out.println(Arrays.toString(primes));
    }
}
```
Output :
[2, 3, 5, 7, 11, 13, 17, 19, 23]