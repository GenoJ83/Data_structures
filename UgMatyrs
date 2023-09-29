def read_uganda_martyrs_file(file_path):
    try:
        with open(file_path, 'r', encoding='utf-8') as file:
            names = [line.strip() for line in file.readlines()]
        return names
    except FileNotFoundError:
        print(f"Error: File '{file_path}' not found.")
        return []

def is_uganda_martyr_name(input_string, file_path):
    # Get the list of Uganda Martyrs' names from the file
    uganda_martyrs_names = read_uganda_martyrs_file(file_path)

    # Convert the input string to lowercase for case-insensitive comparison
    input_string = input_string.lower()

    # Check if the input string matches any of the Uganda Martyrs' names
    for name in uganda_martyrs_names:
        if input_string == name.lower():
            return True

    return False

# Example usage with the correct file path
file_path = r'E:\BsCs\Python\Data Structures\Data_structures\names.txt'
input_name = input("Please enter a name: ")
result = is_uganda_martyr_name(input_name, file_path)

if result:
    print(f"{input_name} is a Uganda Martyr.")
else:
    print(f"{input_name} is not a Uganda Martyr.")
