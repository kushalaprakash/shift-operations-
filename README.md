# shift-operations-
def left_shift(binary, positions):
    print("Original:", binary)

    for i in range(positions):
        binary = binary[1:] + "0"
        print("After left shift", i + 1, ":", binary)

    return binary


def right_shift(binary, positions):
    print("Original:", binary)

    for i in range(positions):
        binary = "0" + binary[:-1]
        print("After right shift", i + 1, ":", binary)

    return binary


# a) Logical left shift of 10110110 by 2 positions
print("a) Logical Left Shift")
result1 = left_shift("10110110", 2)
print("Final Result:", result1)

print()

# b) Logical right shift of 11010100 by 2 positions
print("b) Logical Right Shift")
result2 = right_shift("11010100", 2)
print("Final Result:", result2)