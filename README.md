# Currency Converter App

This React application is a currency converter that allows users to convert amounts between different currencies. It fetches currency exchange rate data from an external API and provides a user-friendly interface for seamless conversions.
#Link
-https://currency-converter-zeta-ashen.vercel.app-

# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

## Expanding the ESLint configuration

If you are developing a production application, we recommend using TypeScript and enable type-aware lint rules. Check out the [TS template](https://github.com/vitejs/vite/tree/main/packages/create-vite/template-react-ts) to integrate TypeScript and [`typescript-eslint`](https://typescript-eslint.io) in your project.


## Features

* **Real-time Currency Conversion:** Converts amounts between various currencies using up-to-date exchange rates.
* **Currency Selection:** Users can select the "from" and "to" currencies from a dropdown list.
* **Amount Input:** Users can enter the amount to be converted.
* **Swap Currencies:** A "Swap" button allows users to quickly switch the "from" and "to" currencies.
* **Responsive Design:** The app is styled with Tailwind CSS for a clean and responsive user interface.

## Technologies Used

* **React:** JavaScript library for building user interfaces.
* **Tailwind CSS:** Utility-first CSS framework for rapid UI development.
* **Custom Hooks:** `useCurrencyInfo` custom hook to fetch and manage currency exchange rate data.

## Getting Started

### Prerequisites

* Node.js and npm (Node Package Manager) installed on your system.

### Installation

1.  Clone the repository to your local machine:

    ```bash
    git clone <repository_url>
    ```

2.  Navigate to the project directory:

    ```bash
    cd <project_directory>
    ```

3.  Install the dependencies:

    ```bash
    npm install
    ```

### Running the Application

1.  Start the development server:

    ```bash
    npm run dev
    ```

2.  Open your browser and navigate to `http://localhost:3000` to view the application.

## Usage

1.  **Select "From" Currency:** Choose the currency you want to convert from using the first dropdown.
2.  **Enter Amount:** Input the amount you want to convert in the input field.
3.  **Select "To" Currency:** Choose the currency you want to convert to using the second dropdown.
4.  **View Converted Amount:** The converted amount will be displayed in the second input field.
5.  **Swap Currencies:** Click the "Swap" button to switch the "from" and "to" currencies.
6.  **Convert:** Click the convert button to convert the amount.

## Code Explanation

* **`App.js`:**
    * Manages the application's state, including the input amount, selected currencies, and converted amount.
    * Uses the `useCurrencyInfo` custom hook to fetch currency exchange rate data.
    * Provides functions for converting amounts and swapping currencies.
    * Renders the `InputBox` components and other UI elements.
* **`InputBox.js`:**
    * A reusable input component for entering amounts and selecting currencies.
    * Receives props for label, amount, currency options, selected currency, and event handlers.
    * Uses the `useId` hook to generate unique IDs for accessibility.
* **`useCurrencyInfo.js`:**
    * Custom hook that fetches currency exchange rate data from an external API.
    * Handles data fetching and error handling.
    * Returns the currency exchange rate data.

## Contributing

Contributions are welcome! If you have any improvements or bug fixes, please submit a pull request.

