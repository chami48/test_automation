# Chat Translator Test Automation Project

## Overview

This project automates testing of the **Pixelssuite Chat Translator** web application using Python and Playwright.
The automation script reads Singlish test cases from an Excel file, sends them to the translator, waits for the translated output, and validates the results against the expected output.

This repository was created as part of the **Software Quality Assurance / Test Automation assignment**.

---

## Target Application

https://www.pixelssuite.com/chat-translator

---

## Project Structure

test_automation
│
├── test_automation.py
├── Assignment 1 - Test cases.xlsx
├── README.md

---

## Prerequisites

Before running the tests, make sure the following software is installed:

* Python 3.8 or higher
* Google Chrome browser
* Internet connection

---

## Step 1 — Install Dependencies

Open a terminal inside the project folder and run:

pip install playwright pandas openpyxl

Then install the required browser for Playwright:

playwright install

---

## Step 2 — Run the Test Automation

Execute the following command in the terminal:

py test_automation.py --excel "Assignment 1 - Test cases(IT23848184).xlsx" --sheet "TestCases" --input-col "Input" --expected-col "Expected output" --url "https://www.pixelssuite.com/chat-translator" --wait-ms 5000 --type-delay-ms 80 --slow-mo-ms 200 --save-every 1 --keep-open

---

## Command Parameters

--excel
Specifies the Excel file containing test cases.

--sheet
Name of the worksheet containing test data.

--input-col
Column that contains Singlish input text.

--expected-col
Column that contains expected translated output.

--url
Web application URL to test.

--wait-ms
Time to wait for translation results in milliseconds.

--type-delay-ms
Typing delay between characters.

--slow-mo-ms
Slows down browser actions for visibility.

--save-every
Saves results after processing each test case.

--keep-open
Keeps the browser open after execution.

---

## Expected Output

The automation will:

* Open the Chat Translator website
* Enter Singlish text from the Excel file
* Capture the translated output
* Compare it with the expected result
* Save the results automatically

---

## Repository Access Requirement

This repository must be set to **Public** so that it can be accessed during marking.

Repositories that cannot be accessed during marking will not be evaluated.

---

## Author

Student Name: Chamya N D
Registration Number: IT23848184
