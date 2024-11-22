# Function Definition

This repository includes the definition and analysis of the mathematical function:

\[
f(x) = 11 + e^{-x}
\]

## Explanation

- **\(11\):** A constant added to the result of the exponential term.
- **\(e^{-x}\):** The exponential function with a negative exponent \(x\). This term decreases as \(x\) increases.

### Properties

1. **Asymptote:**  
   As \(x \to \infty\), \(f(x)\) approaches 11.
   
2. **Behavior at \(x = 0\):**  
   \(f(0) = 11 + e^0 = 11 + 1 = 12\).

3. **Decreasing Function:**  
   \(f(x)\) decreases as \(x\) increases due to the exponential decay term.

### Applications

This function can be applied in various domains, such as:
- **Modeling exponential decay:** For phenomena that include decay over time with a constant offset.
- **Signal processing:** When dealing with decaying signals.
- **Physics and Engineering:** In systems involving a steady-state offset and transient decay.

## Example Plot

Below is an example plot of \(f(x)\) for \(x \in [0, 5]\):

```python
import numpy as np
import matplotlib.pyplot as plt

# Define the function
def f(x):
    return 11 + np.exp(-x)

# Generate x values
x = np.linspace(0, 5, 100)
y = f(x)

# Plot the function
plt.plot(x, y, label=r"$f(x) = 11 + e^{-x}$")
plt.title("Plot of f(x)")
plt.xlabel("x")
plt.ylabel("f(x)")
plt.legend()
plt.grid()
plt.show()
