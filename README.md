# Bubble_Sorting_Kotlin
Сортировка Пузырьком на Котлине

fun main() {
        val sort: (Array<Int>) -> Array<Int> = {
            for (i in it.size - 2 downTo 0) {
                for (j in 0..i) {
                    if (it[j] < it[j + 1]) {
                        val temp = it[j]
                        it[j] = it[j + 1]
                        it[j + 1] = temp
                    }
                }
            }
            it
        }
        val sortedArray = sort(arrayOf(5,-7,6,4,-9,-1,7,5,-3))
        for (i in sortedArray) {
            println(i)
        }
    }
