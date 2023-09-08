[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-718a45dd9cf7e7f842a935f5ebbe5719a5e09af4491e668f4dbf3b35d5cca122.svg)](https://classroom.github.com/online_ide?assignment_repo_id=11786963&assignment_repo_type=AssignmentRepo)
# Mystery Function

What does the `mystery()` function in the following piece of code do? Add your
answer to this markdown file.

```javascript
function mystery(a) {
    if(a.length == 1) return a[0];
    var foo = mystery(a.slice(1, a.length))
    if(foo > a[0]) return foo;
    else return a[0];
}
```

mystery() takes a string as an argument and returns the first character if it's the only character in the string. It then recursively slices the string such that it removes the first character of the string until all that's left is the last character of the string. This last character is stored in variable foo which is then compared to the first character of the string. If foo (the last character) is greater than the first, the function returns foo. Otherwise it returns the first character.
