# 🎓 Assignment: Roman Numeral Toolkit using HashMap, HashSet & Iterator

## 🧠 Objective

Design a **Roman Numeral Toolkit** that:

* Converts numbers to Roman numerals
* Ensures uniqueness using a `HashSet`
* Iterates over converted results using an `Iterator`

This exercise will reinforce:

* Lookup via `HashMap`
* Deduplication via `HashSet`
* Traversal via `Iterator`

---

## 🏛 Scenario

> You're building a **utility for a museum** that prints plaques for Roman artifacts. Visitors can enter multiple numbers (e.g., years or exhibit numbers), but you want to:
>
> 1. Convert them to Roman numerals
> 2. Ensure no duplicates
> 3. Display each result in the order they were processed

---

## 🪜 Step-by-Step Guide

### ✅ Step 1: Create a Class Called `RomanNumeralConverter`

1. Define a private `HashMap<Integer, String>` to store integer-to-Roman mappings.
2. Populate the map with the usual Roman numeral rules.
3. Add a method:

   * `String convertToRoman(int num)`
   * This method should use the map and descending integer keys to build the Roman numeral.

> 🎯 *Goal:* Use `HashMap` for fast lookup of Roman symbols and implement ordered logic separately.

---

### ✅ Step 2: Create a Class Called `RomanConversionTracker`

This class will track **unique conversions** and allow iteration.

1. Declare a private `HashSet<String>` to store **converted Roman numerals**.

   * This prevents duplicate Roman numerals from being stored.
2. Add a method:

   * `void addRoman(String roman)`
   * Only adds it if it doesn’t already exist (Hint: HashSet does this naturally).
3. Add another method:

   * `Iterator<String> getIterator()`
   * This should return an iterator over the `HashSet`.

> 🎯 *Goal:* Learn how HashSet automatically filters duplicates and enables set-based logic.

---

### ✅ Step 3: Bring It Together in a Main Class (`RomanNumeralApp` or similar)

1. Accept a sample list of integers (you can hardcode it for simplicity: `List.of(2, 5, 5, 10, 12, 12)`).
2. For each number:

   * Convert it to a Roman numeral using `RomanNumeralConverter`
   * Add it to `RomanConversionTracker`
3. Use the `Iterator` to loop through and print each unique Roman numeral.

> 🎯 *Goal:* Practice collection iteration using `Iterator<String>` rather than enhanced for-loops.

---

## 🧪 Bonus Testing Suggestions

* Write unit tests using **JUnit 5** for each class
* Assert that duplicates are filtered correctly
* Validate correct Roman numeral outputs

---

## 🧾 Deliverables

Each student must submit:

* All three classes (`RomanNumeralConverter`, `RomanConversionTracker`, `Main/App` class)
* A set of **JUnit 5 test cases**
* A short comment block in the main class explaining how HashMap, HashSet, and Iterator were used

---

## 🧠 Learning Outcome Recap

By the end of this assignment, you will:

* Know when to use a `HashMap` for mapping and lookup
* Understand `HashSet` for deduplication
* Use an `Iterator` for collection traversal in a safe, controlled way


---

## 📚 Java Collections Framework Resources

### ✅ HashMap

* **Oracle Java Docs – HashMap**
  [https://docs.oracle.com/javase/8/docs/api/java/util/HashMap.html](https://docs.oracle.com/javase/8/docs/api/java/util/HashMap.html)

* **Baeldung Guide to HashMap**
  [https://www.baeldung.com/java-hashmap](https://www.baeldung.com/java-hashmap)

---

### ✅ HashSet

* **Oracle Java Docs – HashSet**
  [https://docs.oracle.com/javase/8/docs/api/java/util/HashSet.html](https://docs.oracle.com/javase/8/docs/api/java/util/HashSet.html)

* **GeeksForGeeks – HashSet in Java**
  [https://www.geeksforgeeks.org/hashset-in-java/](https://www.geeksforgeeks.org/hashset-in-java/)

---

### ✅ Iterator

* **Oracle Java Docs – Iterator Interface**
  [https://docs.oracle.com/javase/8/docs/api/java/util/Iterator.html](https://docs.oracle.com/javase/8/docs/api/java/util/Iterator.html)

* **Baeldung – How to Use an Iterator in Java**
  [https://www.baeldung.com/java-iterator](https://www.baeldung.com/java-iterator)

---

## 🏛 Roman Numeral Rules

* **MathWorld – Roman Numerals**
  [https://mathworld.wolfram.com/RomanNumerals.html](https://mathworld.wolfram.com/RomanNumerals.html)

* **Wikipedia – Roman Numerals**
  [https://en.wikipedia.org/wiki/Roman\_numerals](https://en.wikipedia.org/wiki/Roman_numerals)

---

## ⚙️ Tools & Testing Resources

### ✅ Maven

* **Apache Maven in 5 Minutes**
  [https://maven.apache.org/guides/getting-started/maven-in-five-minutes.html](https://maven.apache.org/guides/getting-started/maven-in-five-minutes.html)

### ✅ JUnit 5

* **Official JUnit 5 User Guide**
  [https://junit.org/junit5/docs/current/user-guide/](https://junit.org/junit5/docs/current/user-guide/)

* **Baeldung – Intro to JUnit 5**
  [https://www.baeldung.com/junit-5](https://www.baeldung.com/junit-5)



