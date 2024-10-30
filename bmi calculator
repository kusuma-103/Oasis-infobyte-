def calculate_bmi(weight, height):
  """Calculates the Body Mass Index (BMI) given weight in kilograms and height in meters.

  Args:
    weight: Weight in kilograms.
    height: Height in meters.ṇ

  Returns:
    The calculated BMI.
  """

  bmi = weight / (height ** 2)
  return bmi

def interpret_bmi(bmi):
  """Interprets the BMI value and returns a corresponding health category.

  Args:
    bmi: The calculated BMI.

  Returns:
    A string indicating the health category.
  """

  if bmi < 18.5:
    return "Underweight"
  elif 18.5 <= bmi < 25:
    return "Normal"
  elif 25 <= bmi < 30:
    return "Overweight"
  else:
    return "Obese"

def main():
  weight = float(input("Enter your weight in kilograms: "))
  height = float(input("Enter your height in meters: "))

  bmi = calculate_bmi(weight, height)
  interpretation = interpret_bmi(bmi)

  print(f"Your BMI is: {bmi:.1f}")
  print(f"Interpretation: {interpretation}")

if __name__ == "__main__":
  main()
