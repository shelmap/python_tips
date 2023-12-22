# Module os

os is a module in Python that provides functions for interacting with the operating system.  
Below is a detailed tutorial with code examples in Python using the os module.  
This tutorial covers basic file and directory operations using the os module.  
Remember that these operations can modify the file system, so be careful and use them wisely.

1. Obtaining information about the current directory:
```python
import os

current_directory = os.getcwd()
print(f"Current Directory: {current_directory}")
```

2. Create a new directory:
```python
import os

new_directory = "example_directory"
os.mkdir(new_directory)
print(f"Directory '{new_directory}' created.")

3. List of files and directories in the current directory:
```python
import os

files_and_directories = os.listdir()
print(f"Files and Directories in Current Directory: {files_and_directories}")
```

4. Renaming a file or directory:
```python
import os

old_name = "old_file.txt"
new_name = "new_file.txt"
os.rename(old_name, new_name)
print(f"{old_name} renamed to {new_name}")
```

5. Deleting a file:
```python
import os

file_to_delete = "file_to_delete.txt"
os.remove(file_to_delete)
print(f"{file_to_delete} deleted.")
```

6. Removing a directory:
```python
import os

directory_to_delete = "directory_to_delete"
os.rmdir(directory_to_delete)
print(f"Directory '{directory_to_delete}' deleted.")
```

7. Checking the existence of a file or directory:
```python
import os

file_or_directory = "check_file.txt"
if os.path.exists(file_or_directory):
     print(f"{file_or_directory} exists.")
else:
     print(f"{file_or_directory} does not exist.")
```

8. Building paths to files and directories:
```python
import os

base_path = "/path/to/base"
file_name = "example.txt"
full_path = os.path.join(base_path, file_name)
print(f"Full Path: {full_path}")
```
