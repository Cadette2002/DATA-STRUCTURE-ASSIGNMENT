import array

# Integers: Quantities of tools checked out
tool_quantities = [8, 15, 6, 10, 12, 9, 11]  # Example quantities for different tools

total_checked_out = sum(tool_quantities)
average_checked_out = total_checked_out / len(tool_quantities)
min_checked_out = min(tool_quantities)
max_checked_out = max(tool_quantities)

# Strings: Formatted report using f-strings
report = (
    f"Workshop Tool Checkout Report\n"
    f"Total Tools Checked Out: {total_checked_out}\n"
    f"Average Checked Out per Tool: {average_checked_out:.2f}\n"
    f"Minimum Checked Out: {min_checked_out}\n"
    f"Maximum Checked Out: {max_checked_out}\n"
)

print(report)

# Booleans: Threshold condition and compound condition
threshold = 10
# Compound condition: average exceeds threshold and max is above threshold
if average_checked_out > threshold and max_checked_out > threshold:
    print("Status: Above Standard")
else:
    print("Status: Below Standard")

# Lists: Maintain, modify, and display a list of tool names
tool_names = ["Hammer", "Screwdriver", "Wrench", "Drill", "Saw", "Pliers", "Chisel"]

print("\nTools before modification:", tool_names)

# Add a new tool
tool_names.append("Tape Measure")

# Remove a tool whose name starts with 'C'
tool_names = [tool for tool in tool_names if not tool.startswith('C')]

# Sort and display the list
tool_names.sort()
print("Tools after modification and sorting:", tool_names)

# Arrays: Store fixed-size subset and compare sum
subset_array = array.array('i', tool_quantities[:5])  # First five quantities

array_sum = sum(subset_array)
list_sum = sum(tool_quantities[:5])

print(f"\nSum of array subset: {array_sum}")
print(f"Sum of list subset: {list_sum}")
print("Array and list sums are equal?" , array_sum == list_sum)

# Dictionaries: List of records
tool_records = [
    {"id": 1, "name": "Hammer", "value": 8},
    {"id": 2, "name": "Screwdriver", "value": 15},
    {"id": 3, "name": "Wrench", "value": 6},
    {"id": 4, "name": "Drill", "value": 10},
    {"id": 5, "name": "Saw", "value": 12},
]

# Update record for 'Drill'
for record in tool_records:
    if record["name"] == "Drill":
        record["value"] = 13  # Updated value

# Delete record for 'Wrench'
tool_records = [record for record in tool_records if record["name"] != "Wrench"]

# Compute total 'value' across all records
total_value = sum(record["value"] for record in tool_records)

print("\nTool Records after update and delete:")
for record in tool_records:
    print(record)
print(f"Total 'value' across all records: {total_value}")