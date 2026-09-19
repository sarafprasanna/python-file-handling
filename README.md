# python-file-handling

# Count, Extract, and Write

with open("input.txt", "r") as file:
    lines = file.readlines()

# Count total lines
line_count = len(lines)

# Extract first two lines
first_two_lines = lines[:2]

# Write first two lines to output file
with open("output.txt", "w") as file:
    file.writelines(first_two_lines)

# Display results
print("Total number of lines:", line_count)
print("First two lines:")

for line in first_two_lines:
    print(line, end="")
