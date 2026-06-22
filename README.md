
# Simple Interest Calculator

## Description
This repository contains a simple interest calculator script. Simple interest is a quick and easy method of calculating the interest charge on a loan or investment. It is determined by multiplying the initial principal amount by the interest rate and the time period.

## Formula
The mathematical formula to calculate simple interest is:

**I = P * R * T**

Where:
* **I** = Interest amount
* **P** = Principal amount (the initial amount of money)
* **R** = Annual interest rate (in decimal format)
* **T** = Time (in years)

## Example Calculation
Let's say you invest **$1,000** at an annual interest rate of **5%** for **3 years**.

* P = 1000
* R = 0.05 (which is 5 / 100)
* T = 3

Calculation:
`1000 * 0.05 * 3 = 150`

The simple interest accumulated after 3 years would be **$150**.

## Code Snippet
This project uses a Bash script (`simple-interest.sh`) to perform the calculation automatically. Here is a snippet demonstrating its core functionality:

```bash
#!/bin/bash
# A simple script to calculate simple interest

echo "Enter the principal:"
read p
echo "Enter rate of interest per year:"
read r
echo "Enter time period in years:"
read t

# Calculate simple interest
s=$(echo "$p * $t * $r / 100" | bc)

echo "The simple interest is: "
echo $s
