# Given data
lower <- c(1, 5, 15, 20, 50, 80)
upper <- c(5, 15, 20, 50, 80, 110)
freq <- c(200, 450, 300, 1500, 700, 44)

# Total frequency
N <- sum(freq)
half <- N / 2

# Cumulative frequency
cf <- cumsum(freq)

# Find median class
i <- which(cf >= half)[1]

L <- lower[i]
f <- freq[i]
h <- upper[i] - lower[i]

if (i == 1) {
  cf_before <- 0
} else {
  cf_before <- cf[i - 1]
}

# Calculate median
median <- L + ((half - cf_before) / f) * h

# Display output
cat("Total Frequency:", N, "\n")
cat("Median Class:", L, "-", upper[i], "\n")
cat("Approximate Median:", round(median, 2), "\n")
