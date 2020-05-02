the theory behind the third problem is that: instead of doing dp based on values, we do dp based on the state of shifts. In other words, which shifts should be occupied. We use a binary number to represent the state, for example, 110110 means we take the first,second, the fourth and the fifth shift. We know that many states contribute to the same general mask:  for example, 1101 and 1001 both contribute to the 1000 mask. In order to know how many states contribute to a general mask, we sum up the number of states by digits. Namely, starting from the least significant bit and moving towards the most significant bit, we find numbers that differ by 1 bit, and add the dp value of the greater number to the dp value of the smaller number. This way a state change of multiple bits, (for example, the change from 11 to 00 is a two-bit change, 111 to 000 is three-bit change), is only added once instead of multiple times. 