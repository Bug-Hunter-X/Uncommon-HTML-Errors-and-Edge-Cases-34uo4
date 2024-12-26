# Uncommon HTML Errors and Edge Cases

This repository showcases some less common errors that can occur in HTML, particularly those related to element access, attribute handling, and unexpected null values.  The examples are designed to highlight potential pitfalls and provide solutions for cleaner, more robust code.

## Bugs

* **Accessing Non-Existent Attributes:** Attempting to access an attribute that does not exist on an element will result in `null`. While not an error in itself, subsequent operations on `null` can lead to runtime errors.
* **Method Calls on Null Elements:** Calling methods on elements that do not exist (e.g., due to incorrect IDs) will cause errors.
* **Modifying Read Only Attributes:** Some HTML attributes are read-only, and attempting to modify them after initial assignment will have no effect and might be ignored by the browser.

## Solutions

The solutions focus on robust error handling and best practices for interacting with the DOM.  This includes explicit null checks before performing operations on elements and careful consideration of attribute read-only properties.
