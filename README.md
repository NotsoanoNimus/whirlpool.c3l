# whirlpool.c3l
A C3 library implementation of the WHIRLPOOL hashing algorithm with associated tests.


## Usage
Simply clone the library to your C3 project's `lib/` folder and import `whirlpool` in your project files.

```c3
import whirlpool;

// ...

fn void? verify_input_file(char[] incoming_file_data)
{
    char[] expected_hash = x'1234abcd ...';

    if (whirlpool::hash(incoming_file_data)![..] != expected_hash) return FILE_HASH_MISMATCH?;

    // ...
}
```
