# 🐍 Intro to Python

## Part 1: Cloning the Challenge Repository 🛠️

1. **Clone the Repository**:
   - 🌐 Open your terminal (Command Prompt, PowerShell, Terminal, etc.).
   - 📂 Navigate to the directory where you want to store your project.
   - 🚀 Clone the repository from the GitHub link provided by the SoC coaches (https://github.com/1alexc/soc-challenge-intro-to-python)
   - 🔗 This will create a directory called `soc-challenge-intro-to-python` with the README.md containing instructions.

2. **Navigate to the Project Directory**:
   - Use the following command to move into the newly cloned project directory:
     ```bash
     cd soc-challenge-intro-to-python
     ```

## Part 2: Writing Your First Python Script ✏️

1. **Create a Python File**:
   - 📂 In the project directory, open your text editor (We will be using VS Code, but this will work with other IDEs).
   - 📝 Create a new file and name it `hello_world.py`.

2. **Write a Simple Script**:
   - In `hello_world.py`, write the following code:
     ```python
     def hello():
         return "Hello, World!"
     ```

3. **Run Your Script**:
   - 💾 Save your file.
   - 🔗 Open your terminal and ensure you are still in the project directory.
   - 🚀 Run the script by typing:
     ```bash
     python hello_world.py
     ```
   - If no errors appear, your script is ready!

## Part 3: Understanding the Code 🧠

1. **Breaking It Down**:
   - The `def hello():` line defines a function named `hello`.
   - The `return "Hello, World!"` line tells the function to send back the text "Hello, World!" when it's called.

2. **Calling the Function**:
   - To see the output of this function, add the following line at the end of your script:
     ```python
     print(hello())
     ```
   - 💾 Save the file and run it again in your terminal. You should see the output: `Hello, World!`.

## Part 4: Writing a Simple Test ✅

1. **Why Testing?**:
   - 🛡️ Testing helps us ensure that our code works as expected. Let's write a simple test to check if our `hello()` function is correct.

2. **Create a Test File**:
   - 📂 In your text editor, create a new file in the same project directory called `test_hello.py`.

3. **Write the Test**:
   - In `test_hello.py`, write the following code:
     ```python
     from hello_world import hello  # This imports the hello function from your other file

     def test_hello():
         assert hello() == "Hello, World!"  # This checks if the function returns the correct value

     if __name__ == "__main__":  # __name__ is a special built-in variable in Python. When a Python script is run, the Python interpreter sets this variable. If the script is being run directly (for example, by typing python script.py in the terminal), __name__ is set to "__main__".
         test_hello()
         print("Test passed!")
     ```

4. **Understanding the Test**:
   - The line `assert hello() == "Hello, World!"` checks if the `hello()` function returns "Hello, World!".
   - If the test passes, you'll see "Test passed!" in your terminal.

5. **Run the Test**:
   - 💾 Save `test_hello.py`.
   - 🚀 In your terminal, run the test by typing:
     ```bash
     python test_hello.py
     ```
   - If everything is correct, you should see the message "Test passed!" ✅. If not, double-check your code.

## Part 5: Submitting Your Work 📤

1. **Add Your Changes**:
   - Use Git to add your changes to the staging area:
     ```bash
     git add .
     ```

2. **Commit Your Work**:
   - Commit your changes with a descriptive message:
     ```bash
     git commit -m "Completed intro to Python challenge"
     ```

3. **Push to Your Repository**:
   - Push your changes to the remote repository:
     ```bash
     git push origin main
     ```
## Part 6: Bonus Task 🎯
1. **Experimenting With Your Test**:
   - Try testing your understanding by changing the function name and/or returning another string in the `hello_world.py` file. Remember, if the function name and/or string in the `test_hello.py` file doesn't match, it will return an error when you run python test_hello.py in your terminal.

---