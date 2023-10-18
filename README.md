# Get data from users in a set and print it
def get_user_data():
    user_data = set()
    while True:
        data = input("Enter some data (or 'done' to exit): ")
        if data == "done":
            break
        user_data.add(data)
    return user_data

def main():
    user_data = get_user_data()
    print("User data: ", user_data)

if __name__ == "__main__":
    main()


    functions = {
    "list": ["append", "clear", "copy", "count", "extend", "index", "insert", "pop", "remove", "reverse", "sort"],
    "dictionary": ["clear", "copy", "fromkeys", "get", "items", "keys", "pop", "popitem", "setdefault", "update", "values"],
    "set": ["add", "clear", "copy", "difference", "difference_update", "discard", "intersection", 
            "intersection_update","isdisjoint","issubset","issuperset","pop","remove","symmetric_difference",
            "symmetric_difference_update","union","update"],
    "tuple": ["count","index"]
}

for key in functions:
    print(f"{key.capitalize()} functions: {functions[key]}")
