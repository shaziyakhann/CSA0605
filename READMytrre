def generate_subsets_with_target(E, target):
    result = []
    
    def backtrack(start, path):
        # If the current subset contains the target element, append it to the result
        if target in path:
            result.append(path[:])  # Append a copy of path
        
        for i in range(start, len(E)):
            # Include E[i] in the current subset
            path.append(E[i])
            # Move on to the next element
            backtrack(i + 1, path)
            # Backtrack: remove the last element added
            path.pop()

    backtrack(0, [])
    return result

# Example usage:
E = [2, 3, 4, 5]
target = 3
subsets = generate_subsets_with_target(E, target)
print(subsets)
