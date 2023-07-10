# Minigrep

Minigrep is a simplified version of the grep command line tool implemented in Rust.

It allows you to search for a specified term within a given file. The program supports both case-sensitive and case-insensitive search, depending on the value of the IGNORE_CASE environment variable.

## Usage

To run the program, use the following command:

```
cargo run -- [term] [file]
```

Replace `[term]` with the term you want to search for, and `[file]` with the path to the file in which you want to search.

If you want the search to be case-insensitive, set the environment variable IGNORE_CASE to 1 before running the program.

```
$ IGNORE_CASE=1 cargo run -- [term] [file]
```
Or, if you are running on Windows:
```
PS> $Env:IGNORE_CASE=1; cargo run -- [term] [file]
```


## Example

Suppose you want to search for the term "hello" in a file named "example.txt" and perform a case-insensitive search. Here's how you would run the program:

```
IGNORE_CASE=1 cargo run -- hello example.txt
```

The program will display the lines in the file that contain the specified term.

## License

This program is open source and distributed under the MIT License. See the [LICENSE](LICENSE) file for more details.

Feel free to modify the README file to suit your specific requirements and add any additional information or sections as needed.
