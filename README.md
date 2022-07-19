import json

# json_data = 
# '[{"Gender": "Male", "HeightCm" :171, "WeightKg": 96},{"Gender": "Male", "HeightCm" :171, "WeightKg": 96}]'

# data = json.loads(json_data)
# print(data)

mass = 47
height = 1.63

BMI = mass/height**2
if(BMI <= 18.4):
	category = "Underweight"
	risk = "Malnutrition risk"
elif(BMI <24.9):
	category = "Normal weight"
	risk = "Low risk"
elif(BMI < 29.9):
	category = "Overweight"
	risk = "Enhanced risk"
elif(BMI < 34.9):
	category = "Moderately obese"
	risk = "Medium risk"
elif(BMI < 39.9):
	category = "Severely obese"
	risk = "High risk"
else:
	category = "Very severely obese"
	risk = "Very high risk"

print(BMI)
print(category)
print(risk)
