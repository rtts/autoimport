## 0.3.0 (2020-12-17)

### Feat

- Add imports of the local package objects
- make autoimport manage the commonly used imports

### Refactor

- move the business logic to the SourceCode entity

### fix

- remove all unused imports instead of just one

## 0.2.2 (2020-12-11)

### Fix

- remove unused imported objects in multiline from import statements

## 0.2.1 (2020-12-10)

### Fix

- support multiline import statements and multiline strings

## 0.2.0 (2020-11-12)

### Feat

- move import statements to the top

### Fix

- **setup.py**: extract the version from source without exec statement

## 0.1.1 (2020-10-27)

### Fix

- correct the formatting of single line module docstrings.
- add newline between module docstring, import statements and code.

## 0.1.0 (2020-10-23)

### Feat

- create first version of the program (#3)
- create initial project structure