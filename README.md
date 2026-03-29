# Python Algorithm for File Updates (IP Allow List)

## Project Description
In this project, I developed a Python algorithm to manage access to restricted content. The organization uses an "allow list" to control access to sensitive data. I automated the process of removing unauthorized IP addresses from this list to improve security efficiency.

## Skills Demonstrated
* **Python Programming:** File handling, loops, and conditional logic.
* **Security Automation:** Streamlining access control tasks.
* **Data Parsing:** Converting and filtering string/list data types.

## How it Works
1. **Open and Read:** The script opens `allow_list.txt` using a `with` statement.
2. **Convert to List:** Using `.split()`, the IP addresses are converted from a string to a list for processing.
3. **Filter:** A `for` loop checks each IP against a `remove_list`. If a match is found, the `.remove()` method is applied.
4. **Update File:** The updated list is joined back into a string and overwritten into the original file using the `"w"` parameter.

## Usage
Simply run the script to update your IP allow list:
```python
python update_ip_list.py
