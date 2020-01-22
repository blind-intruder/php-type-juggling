# PHP type juggling

In PHP you can compare two variables using these two methods.
 * Loose comparison ('==' or '!=')
 * Strict comparison ('===' or !==)

## Type juggling
PHP has a feature called “type juggling”, or “type coercion”. This means that during the comparison of variables of different types, PHP will first convert them to a common, comparable type.


### Mitigation

**Loose comparison**
```
$var1 = 7
$var2 = “7”
if ($example_int == $example_str) {
   echo("PHP can compare ints and strings.")
}
```
**Strict Comparison**
```
$var1 = 7
$var2 = “7”
if ($example_int === $example_str) {
   echo("This will return error.")
}
```
