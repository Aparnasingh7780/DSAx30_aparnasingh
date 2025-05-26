def print_pattern(N):
    for i in range(1, N + 1):
        # Generate the first half of the pattern (A to ith character)
        first_half = ''.join(chr(ord('A') + j) for j in range(i))
        # Generate the second half (reverse of the first half minus last character)
        second_half = first_half[:-1][::-1]
        # Combine and print the result
        print(first_half + second_half)

# Example usage:
N = int(input("Enter N: "))
print_pattern(N)
