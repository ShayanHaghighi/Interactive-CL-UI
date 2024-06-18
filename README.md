# Terminal Interactive Library

This Python library provides interactive terminal functionalities to enhance user experience in command-line applications. The library includes functions for single and multiple option selection using arrow keys, text input, and text-based option selection.

## Features

1. **Single Option Selection with Arrow Keys**
2. **Multiple Option Selection with Arrow Keys**
3. **Text Input Prompt**
4. **Text-Based Option Selection (e.g., Y/n)**
5. **Yes/No Option Selection**

## Installation

To install the library, clone the repository and navigate to the project directory:

```sh
git clone https://github.com/yourusername/terminal-interactive-library.git
cd terminal-interactive-library
```

## Usage
### 1. Single Option Selection with Arrow Keys

Allows users to select a single option from a set of options using arrow keys.

```python
from interactive-cmd.py import select_option

options = ["Option 1", "Option 2", "Option 3"]
selected_option = select_option("Select an option:", options)
print(f"You selected: {selected_option}")
```


### 2. Multiple Option Selection with Arrow Keys

Allows users to select multiple options from a set of options using arrow keys.

```python
from interactive-cmd.py import select_multiple_options_with_arrows

options = ["Option 1", "Option 2", "Option 3"]
selected_options = select_multiple_options_with_arrows("Select multiple options:", options)
print(f"You selected: {', '.join(selected_options)}")
```

### 3. Text Input Prompt

Allows users to input text given a prompt.

```python

from interactive-cmd.py import input_text

user_input = input_text("Enter your name:")
print(f"Hello, {user_input}!")
```

### 4. Text-Based Option Selection

Allows users to select an option using text input (e.g., Y/n).

```python

from interactive-cmd.py import input_text_with_options

answer = input_text_with_options("What access rights would you like to give ",options="rwxh",default="r")
print(f"You selected: {answer}")
```
### 4. Yes/No Text-Based Option Selection

Allows users to select Y/n using text input.

```python

from interactive-cmd.py import input_yesorno

confirmation = input_yesorno("Add file path",default="y")
print(f"You selected: {confirmation}")
```


## License

This project is licensed under the MIT License. See the LICENSE file for details.
Contributing

## Acknowledgements

Special thanks Philippe on Stack Overflow, whose answer inspired me to write this code.
