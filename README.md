# Simple-White-Noise-Generator
# White Noise Generator in C++

This repository contains a simple class for generating white noise in C++ using a basic pseudorandom number generator.

## Features
- **`NoiseGenerator` Class:** Provides methods to generate white noise values between -1.0 and 1.0.
- **Seed-Based Randomness:** The noise is generated using a seeded pseudorandom algorithm.
  
## Usage

```cpp
#include "NoiseGenerator.h"

int main() {
    NoiseGenerator generator;
    generator.reset();  // Reset the noise seed
    
    // Generate 10 random white noise values
    for (int i = 0; i < 10; i++) {
        float noise = generator.nextValue();
        std::cout << noise << std::endl;
    }
    
    return 0;
}
