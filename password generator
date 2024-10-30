mport random
import string

def generate_password(length=8, include_uppercase=True, include_lowercase=True, include_numbers=True, include_symbols=True):
  """Generates a random password based on the given parameters.

  Args:
    length: The desired length of the password.
    include_uppercase: Whether to include uppercase letters.
    include_lowercase: Whether to include lowercase letters.
    include_numbers: Whether to include numbers.
    include_symbols: Whether to include symbols.

  Returns:
    A randomly generated password string.
  """

  characters = ''
  if include_uppercase:
    characters += string.ascii_uppercase
  if include_lowercase:
    characters += string.ascii_lowercase
  if include_numbers:
    characters += string.digits
  if include_symbols:
    characters += string.punctuation

  if not characters:
    raise ValueError("At least one character type must be selected.")

  password = ''.join(random.choice(characters) for _ in range(length))
  return password

if __name__ == "__main__":
  password = generate_password(12, True, True, True, True)
  print(password)
