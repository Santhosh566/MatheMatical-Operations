"# MatheMatical-Operations" 
# Mathematical Calculator Web Application
This project is a simple mathematical calculator built using Django. It provides basic operations such as addition, subtraction, multiplication, and division. The application also includes a background image that can be customized, providing a visually appealing interface for users.

## Features
- Basic mathematical operations: Addition, Subtraction, Multiplication, and Division.
- Responsive design, ensuring proper display across devices.
- Uses Django's templating engine to render the form and display results.
- Background image displayed on the calculator page for a better user experience.

## Project Structure

### 1.Static Folder
   - The `static` folder contains the images used in the application. The calculator page background image is stored under `static/calculator/images/`.

### 2. Templates Folder
   - The `index.html` file is located inside the templates folder (`templates/calculator/index.html`) and contains the structure of the web page.

### 3. Views (views.py)
   - `views.py` handles the logic of rendering the calculator page and processing the submitted values for calculation.
   - The `index` view renders the HTML form for input and `calculate` processes the calculation based on the user-selected operation.

## Setup and Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/your-repository-name/calculator-app.git
    ```

2. Install dependencies:
    Make sure you have Django installed:
    ```bash
    pip install django
    ```

3. Run the Django development server:
    ```bash
    python manage.py runserver
    ```

4. Access the app:
    Open your browser and navigate to:
    ```
    http://127.0.0.1:8000/
    ```

## How to Use

1. On the homepage, you will see input fields for two numbers and buttons for different operations: ADD, SUB, MUL, and DIV.
2. Enter the numbers you want to calculate and click on one of the operation buttons.
3. The result will be displayed on the same page below the input fields.

## Code Explanation

In the `index.html` file, the background image is referenced in the following line:

```html
background-image: url("{% static 'calculator/images/image.jpg' %}");
```

This line inserts the background image (`image.jpg`) located in the `static/calculator/images/` folder.

The mathematical operations (ADD, SUB, MUL, DIV) are handled in the `views.py` file:

```python
if operation == 'ADD':
    result = num1 + num2
elif operation == 'SUB':
    result = num1 - num2
elif operation == 'MUL':
    result = num1 * num2
else:
    result = num1 / num2
```

These conditions check the user's selected operation and perform the respective mathematical calculation.
## User Interface
![Screenshot 2025-01-10 083312](https://github.com/user-attachments/assets/ff875b45-0f27-4934-b360-912ad3dbd4de)

## Conclusion

This project serves as a simple calculator web application with a responsive design, providing basic arithmetic operations and a stylish background image. You can further extend this by adding more advanced features or improving the UI.


