# OPSL OpenSouceLanguage
OPSL is a language program in Python.

# How to Run OPSL files
Go to the folder, open shell.py file, type the file name in the input
Example:
  '''rs
  
  OPSL > RUN("test.opsl")
  
  '''rs


# Codes

Hello World:
  '''rs
  PRINT("Hello World")
  '''rs
loop,spoop:
  '''rs
FUN oopify(prefix) -> prefix + "oop"

FUN join(elements, separator)
	VAR result = ""
	VAR len = LEN(elements)

	FOR i = 0 TO len THEN
		VAR result = result + elements/i
		IF i != len - 1 THEN VAR result = result + separator
	END

	RETURN result
END

FUN map(elements, func)
	VAR new_elements = []

	FOR i = 0 TO LEN(elements) THEN
		APPEND(new_elements, func(elements/i))
	END

	RETURN new_elements
END

PRINT("Greetings universe!")

FOR i = 0 TO 100 THEN
	PRINT(join(map(["l", "sp"], oopify), ", "))
END

  '''rs
