# system that calculates
# 1. Room cost based on the type
# 2.Restaurant bill per day
# 3. Laundry bill 
# 4. Gaming bill per session

# step 1 store what needs to be stored
rooms_types = {
    "one_b": 100,
    "two_b": 150,
    "three_b": 200
}
food_bill = 50

laundry_bill = 40

gaming_session = 15

# step 2, we print to the user
print("Welcome to Utamu billing system")
# Step 3 function declaration
def room_billing(room_type: str, number_days: int) -> float:
    if room_type == "one_b":
        return rooms_types["one_b"]  * number_days
    elif room_type == "two_b":
        return rooms_types["two_b"]  * number_days
    elif room_type == "three_b":
        return rooms_types["three_b"]  * number_days    
    else:
        print("Please enter a valid room name")

def calculate_food(number_meals: int) -> float:
    # print("Calculating food pricing...")
    return food_bill * number_meals


def fcytcfgdd(number_of_times: int) -> float:
    # print("Calculating laundry pricing...")
    return laundry_bill * number_of_times

def gaming_session_bill(sessions: int) -> float:
    # print("Calculating gaming pricing...")
    return gaming_session * sessions

# we input and call the functions
room_billing = room_billing("two_b", 4)
# print("Room costs were $:",room_billing)
print(room_billing)

food_cost = calculate_food(7)
# print(f"Food costs: ${food_cost}")
print(food_cost)

laundry_bill = fcytcfgdd(4)
# print(f"laundry_bill:${laundry_bill}")
print(laundry_bill)

gaming_session_bill = gaming_session_bill(15)
# print(f"gaming_session: $ {gaming_session_bill}")
print(f"Gaming session: $ {gaming_session_bill}")
