##Code Convention Check in Sublime Text 3 with PEP 8
###Install Linter
 1. pep8

 ```
 pip install pep8
 ```

###Install Package
 1. SublimeLinter

 ```
  - Ctrl + Shift + P
  - Type "Install" and Enter
  - Type "SublimeLinter" and Enter
 ```
 2. SublimeLinter-Pep8

 ```
  - Ctrl + Shift + P
  - Type "Install" and Enter
  - Type "SublimeLinter-pep8" and Enter
 ```

###Basic Setting to Start Python
 * Sublime Text 3
  1. Open a .py file
  2. Preference → Setting - More → Syntax User
  3. add
  ```
  {
			"tab_size": 4,
			"translate_tabs_to_spaces": true,
			"trim_trailing_white_space_on_save": true
	}
  ```

Ref: [SublimeLinter-pep8](https://github.com/SublimeLinter/SublimeLinter-pep8)