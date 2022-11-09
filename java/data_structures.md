# Java Data Structures Cheatsheet

## 1) Array
- Basically a lisst of cells/buckets where you define the size(fixed).
- First index is 0.
- Fast for data retrievals. `O(n)`
- Compact memory usage if size is known.
- Delete operations very hard.
- Building block for 2D Array.

```
import java.util.Arrays;

public class TheArrays {
    public static void main(Strings[] args) {
        String[] colors = new String[5];
        colors[0] = "purple";
        colors[1] = "blue";
        System.out.println(Arrays.toString(colors)); // print wole array

        System.out.println(colors[2]);  // print specific element

        int[] numbers = {100, 200}; // faster way to initialize fixed size array

        for (int i = 0;i < colors.length;i++){     // print array normally
            System.out.println(colors[i]);
        }
        for (int i = colors.length - 1;i >= 0;i--){     // print array in reverse
            System.out.println(colors[i]);
        }
        for (String color : colors){    // enhanced for loops
            System.out.println(color);
        }  

        Arrays.stream(colors).forEach(System.out::println);     // printing using array streams
    }
}
```

## 2) 2D - Array
```
public class WorkiingWith2dArrays {
    public static void main(String[] args){
        char[][] board = new char[3][3];
        for(int i=0;i<3;i++){
            for(int j=0;j<3;j++){
                board[i][j] = '-';
            }
        }

        char[][] boardTwo = new char[][] {  // creating 2D array inline
            new char[] {'-','-','-'},
            new char[] {'-','-','-'},
            new char[] {'-','-','-'}
        };
        System.out.println(Arrays.deepToString(board));
    }
}