# balanced_brackets

This Rust code implements a function to determine if a string of brackets is balanced.

A string of brackets is balanced if each opening bracket has a corresponding closing bracket, and the brackets are nested correctly.

The code uses a stack to track the open brackets. When an opening bracket is encountered, it is pushed onto the stack. When a closing bracket is encountered, it is popped off the stack. If the closing bracket does not match the top of the stack, the string is not balanced.

The code also uses a hash map to store the pairs of opening and closing brackets. This allows the code to quickly check if a closing bracket matches an opening bracket.

The code is tested using the `assert_eq!` macro. The tests ensure that the code correctly identifies balanced and unbalanced strings.

## Run

for running tests only you need to execute the next command

```rust
cargo test
```

## Usage

To use the code, simply call the `balanced` function with a string of brackets as input. The function will return `true` if the string is balanced, and `false` otherwise.

For example, the following code will print `true`:

```rust
assert_eq!(balanced("()"), true);
```
