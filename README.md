bouncy.py
initial_height = float(input("Enter the initial height of the ball (in feet): "))
bounciness_index = float(input("Enter the bounciness index: "))
num_bounces = int(input("Enter the number of bounces: "))
total_distance = initial_height
current_height = initial_height
for _ in range(num_bounces):
    total_distance += current_height * bounciness_index * 2
    current_height *= bounciness_index
print("The total distance traveled by the ball is in feet is:", total_distance)

equilateral.py
side1 = float(input("Enter the length of the first side: "))
side2 = float(input("Enter the length of the second side: "))
side3 = float(input("Enter the length of the third side: "))
if side1 == side2 == side3:
    print("The triangle is an equilateral triangle.")
else:
    print("The triangle is not an equilateral triangle.")

population.py
initial_population = int(input("Enter the initial number of organisms: "))
growth_rate = float(input("Enter the growth rate: "))
growth_period = float(input("Enter the number of hours to achieve this growth rate: "))
total_duration = float(input("Enter the total number of hours for population growth: "))
number_of_periods = total_duration / growth_period
final_population = initial_population * (growth_rate ** number_of_periods)
print("The predicted population after:", total_duration, "hours is:", final_population)
