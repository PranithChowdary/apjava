# Hashmaps
<hr>
***Hashmaps*** are helpful tools that allow us to store a key and a value. Unlike Arrays and Arraylists, ***Hashmaps*** allow us to easily look up a value if we know its key. 
<br>
<br>
With that said, let's say you are creating a piece of software that stores student grades for a class. We want to be able to look up a student's grade by their name, so we will need to use a ***Hashmap***.

### What a Hashmap Looks Like
<hr>
With ***Hashmaps*** we assign a ***key*** and a ***value*** associated with that ***key***. If we are creating a piece of software to store student grades, our ***keys*** are the students' names and the ***value*** is the grade. 

This would look like:

| Key | Value |
| --- | --- |
| Wezley Sherman | 85 |
| Wade Adams | 95 |
| Julio Rodriguez | 84 |
| Trevor Forrey | 100 |
| Ada Lovelace | 96 |
| Sally Pants | 98 |
| Sarah Abe | 86 |

The ***Key*** is the element we use to look up a specific ***Value*** in the map.
<br>
The ***Value*** is the result we get when we look up a specific item with a ***Key***. 
<br>
The ***Key-Value Pair*** is the combination of the ***Key*** and the ***Value*** associated.
<br>

It is important to remember that each ***key*** can only have **one** ***value***, and ***key-value pairs*** are **not** ordered.

### Utilizing Hashmaps
<hr>

##### Creating Hashmaps:

In order to create a ***Hashmap*** we use: `Hashmap<key_type, value_type> name = new Hashmap<key_type, value_type>();`. 
<br>
<br>
If we were to create our grade book ***Hashmap*** we would use: 
```Java
Hashmap<String, Integer> gradeBook = new Hashmap<String, Integer>();
```
<br>

##### Adding Items:

To add an item to a ***Hashmap*** we use: `map.put(key, value);`
<br>
<br>
If we were to add grades to our grade book ***Hashmap*** we would use:
```Java
gradeBook.put("Wezley Sherman", 85);
gradeBook.put("Wade Adams", 95);
gradeBook.put("Julio Rodriguez", 84);
...
```
<br>

##### Retrieving Items:

To retrieve an item from a ***Hashmap*** we use: `map.get(key);`
<br>
<br>
Let's say we wanted to access Trevor Forry's and Ada Lovelace's grades. To do so we would use:
```Java
// `adaGrade` would contain `96`
int adaGrade = gradeBook.get("Ada Lovelace");
// `trevGrade` would contain `100`
int trevGrade = gradeBook.get("Trevor Forrey");
```
<br>

##### Iterating Over a Hashmap:

Now, let's say we want to print out every grade in our grade book. In order to do this, we would have to iterate over our ***Hashmap***. Here is an example of what that would look like:

```Java
System.out.println("Class Grades: ");

// For each `key` in gradeBook.keySet()
for(String key: in gradeBook.keySet) 
{
  int grade = gradeBook.get(key);
  System.out.println(key + ": " + grade);
}
```

