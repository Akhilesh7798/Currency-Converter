## Working

This Currency Converter web app enables users to convert an amount from one currency to another with real-time exchange rates and dynamic flag display.

**How it works:**

1. **Currency Dropdowns**:  
   Two dropdown menus allow you to select the source ("from") and target ("to") currencies. Each selection automatically updates the country flag next to it, based on the chosen currency code.

2. **Country Flags**:  
   Flags are displayed using the [FlagsAPI](https://flagsapi.com/) and are dynamically updated whenever a currency is changed.

3. **Amount Input**:  
   Enter the amount you want to convert in the input field. The default is set to "1" if left blank or if a value less than 1 is entered.

4. **Conversion**:  
   - When you click the "Convert" button, the app fetches the latest exchange rate for the selected "from" and "to" currencies using [Fawaz Ahmed’s Currency API](https://github.com/fawazahmed0/currency-api).
   - The exchange rate is applied to the entered amount.
   - The result, showing the converted amount, is displayed below the button in the format:  
     `amount FROM_CURRENCY = converted_amount TO_CURRENCY`

5. **Auto Update on Load**:  
   When the page loads, it automatically converts the default amount (or your last entered amount) with the default currencies (USD to INR).

6. **Responsive & User Friendly**:  
   The UI is clean, centered, and works on all device sizes. Buttons provide visual feedback on hover and click.

---

**Note:**  
All operations are performed client-side using JavaScript and fetch requests—no backend needed!
