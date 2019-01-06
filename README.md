# Pathweaver.py
A script for transforming [Pathweaver](https://github.com/wpilibsuite/PathWeaver) output into Java code.

## Getting started

### Dependencies
- Python 3

### Install
To install, clone this repository.

### Usage
Run the script as so, replacing `filename` with the name of your built path csv file, and `classname` with the name of the final class:

```Shell
python3 pathweaver.py filename classname
```

This will print the class to the terminal, to save it to a file, just use the bash stream tools:

```Shell
python3 pathweaver.py filename classname > classname.java
```

This will generate code similar to that shown below:

```Java

public class RightPath {
	// Position, velocity, acceleration, duration
	public static double[][] points = new double[][]{
		{ 0.000198, 0.019807, 0.990342, 0.020000 },
		{ 0.000262, 0.003194, -0.830654, 0.020000 },
		{ 0.000390, 0.006392, 0.159929, 0.020000 },
		{ 0.000582, 0.009601, 0.160412, 0.020000 },
		{ 0.000838, 0.012823, 0.161136, 0.020000 },
		{ 0.004345, 0.175359, 8.126772, 0.020000 },
		{ 0.009484, 0.256936, 4.078885, 0.020000 },
		{ 0.015488, 0.300168, 2.161597, 0.020000 },
    ...
  };
}
```

# Contributing
Please fork this repo and submit a pull request to contribute. I will review all changes and respond if they are accepted or rejected (as well as reasons, so it will be accepted).

## Issues
If you are submitting a bug, please describe the bug in detail and how to replicate if possible. Logs are also very useful.

If you are submitting a feature idea, please describe it in detail and document the potential use cases of that feature if it isn't clear.

# Credits
Just me for now.

# License
You are free to copy, modify, and distribute Pathweaver.py with attribution under the terms of the MIT license. See the [LICENSE](LICENSE) file for details.
