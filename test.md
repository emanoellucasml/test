```kotlin
fun isPalindrome(word: String): Boolean {
   var right: Int = word.size - 1
   var left:  Int = 0
   while (left++ != right--) {
      if (word[left] != word[right]) {
         return false
      }
   }
   return true
}

fun main() {
   val word = "ovo"
   println("Is $word palindrome? ${isPalindrome(word)}")
}
```
