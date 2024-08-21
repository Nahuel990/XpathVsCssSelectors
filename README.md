# XPath vs CSS Selector Performance Test

To excecute just open the HTML file in the browser and check the console

This project includes a comprehensive HTML page to test and compare the performance of XPath and CSS selectors across various scenarios. The HTML page contains examples where XPath and CSS selectors are tested to understand their relative performance.

## HTML Examples

1. **Sibling Element Selection**
   - **XPath Selector:** `//h2/following-sibling::p[1]`
   - **CSS Selector:** `h2 + p`

2. **Attribute Value Containment**
   - **XPath Selector:** `//button[contains(@data-action, 'submit')]`
   - **CSS Selector:** `button[data-action*='submit']`

3. **Last Element in a List**
   - **XPath Selector:** `//ul[@class='items']/li[last()]`
   - **CSS Selector:** `.items li:last-child`

4. **Complex Conditional Logic**
   - **XPath Selector:** `//div[@data-status='active' and @data-role='user']`
   - **CSS Selector:** `.box[data-status='active'][data-role='user']`

5. **Partial Attribute Value**
   - **XPath Selector:** `//input[starts-with(@name, 'user')]`
   - **CSS Selector:** `input[name^='user']`

6. **Simple Element Selection**
   - **XPath Selector:** `//div[@class='box']`
   - **CSS Selector:** `.box`

7. **Select Hidden Elements**
   - **XPath Selector:** `//div[@class='hidden']`
   - **CSS Selector:** `.hidden`

8. **Descendant Selection**
   - **XPath Selector:** `//div[@class='content']//p`
   - **CSS Selector:** `.content p`

## Testing Instructions

1. **Open the HTML File**
   - Open `index.html` in a web browser.

2. **Run JavaScript Performance Tests**
   - The performance tests will run automatically when the page loads.
   - The results will be logged to the browser’s developer console.

3. **View Performance Results**
   - Open the developer console (`F12` or `Ctrl+Shift+I` / `Cmd+Option+I` on Mac).
   - Check the console logs for timing results of each XPath and CSS selector test.

## Notes

- XPath may provide advantages in complex scenarios, such as conditional logic or sibling element selection.
- CSS selectors are typically faster and more efficient for straightforward queries and element selection.
- Performance can vary depending on the browser’s implementation and the complexity of the DOM.

Feel free to modify the HTML and JavaScript code to further explore performance differences and adapt the tests to your specific needs.
