# Documentation development and contributions

1. Variables and functions names must be explicit (no abrevations)
2. Codes lines must not exceed 80 characters and function must not exceed 45 lines
3. No customed security functions are allowed (don't use `os.system`, `exec`, `eval`...), use `html.escape`, `subprocess.call` with `shell=False` ...instead
4. Protect your `form`(formulaires html) with **CSRF token** (you can use WebScripts CSRF tokens) and always harden your **CSP politicy**
5. Styles and JS files must always be imported with an integrity verification (**SHA512**)
6. Docstring for each modules, classes and functions
7. Use WebScripts logs system and add enough logs for the tracability of each functionnalities
8. Write a user documentation (with markdown syntax)

## Python 

1. Your code should contain the following lines in order for you to execute it from your command line

```python 
if __name__ == "__main__":
    exit(main())
```

### Modules


## Scripts

1. Your script must always have an error code (0 for success, 1 to 126 for identified errors, and 127 for unknown errors)
