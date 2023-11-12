# Assignment 6

Serverless development

In this assignment, write a serverless function to fetch questions from any third-party source(s) and populate the question repository (refer Assignment 1 & 2).

We utilized a [third party repository](https://github.com/kyle8998/Practice-Coding-Questions.git) of markdown questions for this assignment. We have a firebase function (serverless logic) that upon an API call trigger, will download markdown files from the third party repository and upload the files based on simple rules (i.e. correct format, can be tagged easily, etc.).

## Steps to replicate

To start, use a suitable application like Postman to trigger requests to the function. Send a POST request to the firebase function URL, with the header `password-header` value set appropriately (see [example](./example.jpg)). Refer to the canvas submission for these details.

If the database is already populated, delete a few of them. E.g.: `Best Time to Buy and Sell Stock`, `Best Time to Buy and Sell Stock II`, `Best Time to Buy and Sell Stock III`, and run the function. You should find the missing questions be populated.
