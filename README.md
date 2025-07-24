
using namespace std;

int main() {
    double num1, num2;
    char operation;
    
    cout << "Simple Arithmetic Calculator" << endl;
    cout << "---------------------------" << endl;
    
    // Get user input
    cout << "Enter first number: ";
    cin  num1;
    
    cout << "Enter second number: ";
    cin  num2;
    
    cout << "Choose operation (+, -, *, /): ";
    cin  operation;
    
    // Perform calculation based on operation
    switch(operation) {
        case '+':
            cout << "Result: " << num1 << " + " << num2 << " = " << num1 + num2 << endl;
            break;
        case '-':
            cout << "Result: " << num1 << " - " << num2 << " = " << num1 - num2 << endl;
            break;
        case '*':
            cout << "Result: " << num1 << " * " << num2 << " = " << num1 * num2 << endl;
            break;
        case '/':
            if(num2 != 0) {
                cout << "Result: " << num1 << " / " << num2 << " = " << num1 / num2 << endl;
            } else {
                cout << "Error: Division by zero is not allowed!" << endl;
            }
            break;
        default:
            cout << "Error: Invalid operation selected!" << endl;
            break;
    }
    
    return 0;
}
