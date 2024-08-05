def access_control(age, has_id, is_member, access_level, country):
    # Use Boolean operators to check conditions
    if age >= 18 and has_id and country in ["USA", "Canada", "UK"]:
        if access_level > 5 or (is_member and access_level >= 3):
            if not (country == "USA" and access_level < 7):
                return "Full access granted."
            else:
                return "Limited access granted due to country restrictions."
        else:
            return "Access denied due to insufficient access level."
    else:
        return "Access denied due to age, lack of ID, or country restriction."

# Test the function
age = int(input("Enter your age: "))
has_id = input("Do you have an ID? (yes/no): ").lower() == 'yes'
is_member = input("Are you a member? (yes/no): ").lower() == 'yes'
access_level = int(input("Enter your access level (1-10): "))
country = input("Enter your country: ")

result = access_control(age, has_id, is_member, access_level, country)
print(result)
