# DevTools - Debugging
1. The error is that the inputs are strings. Instead of doing addition, it is concatenating both strings so the result of num1 + num2 is num1num2.
2. I would convert each input to an integer using the parseInt(). This way it will be able to add integers together.