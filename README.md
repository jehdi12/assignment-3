# assignment-3

import java.util.HashSet;

public class UniqueCharacters {
    public static boolean isAllUnique(String str) {
        
        HashSet<Character> charSet = new HashSet<>();

        
        for (char c : str.toCharArray()) {
           
            if (charSet.contains(c)) {
                return false;
            }
           
            charSet.add(c);
        }

       
        return true;
    }

    public static void main(String[] args) {
        System.out.println(isAllUnique("stack"));   // true
        System.out.println(isAllUnique("unique"));  // false
    }
}
