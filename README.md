WhatsApp Analyser
==================


WhatsApp Analyser is a tool that scans the chats on WhatsApp web to generate reports giving interesting insights into the user's behaviour pattern in group chats. Used python web -application automation library **Selenium** and web scraping library **Beautiful Soup** to automate logging in,scanning group chats to parse the **HTML** and to get a DOM object to extract features such as chats,emojis ,date etc, to perform analysis on. Developed backend in **Node.js** to run the python script and return the responses to the **REST** calls made by **React.js Frontend**. Used **Chart.js** library, to make the React frontend more appealing and infographic.

===================
---

![Chat Preview](https://publicbucketresume.s3.ap-south-1.amazonaws.com/BilateralChart.PNG)
---
##### **** frequency of bilateral talks happening between members of the chat group
===================
---
## `How Does It Work?`

Below is the step by step process to be followed to generate the analysis :)

### Steps :
- The user must intall chrome driver on his machine before procedding further.
- The User enters his whatsapp profile name, the whatsapp groups he wants to analyze,the amount of chats he wants to analyze {Suggested minimum 40}

    ![Chat Preview](https://publicbucketresume.s3.ap-south-1.amazonaws.com/FormPage.PNG)

- The User must also enter the intallation path of chrome driver
- Press the submit button
- The chrome browser will open automatically and direct to whatsapp web page, scan the qr code from your mobile phone to login
- The whatsapp screen wil start scrolling automatically to select the whatsapp group you requested to analyze
- The selenium will scroll through the whatsapp chats automatically, parallely the Beautiful Soup libray will svae the rendered HTML pages to Document Object Model Objects
- By the time the scrolling of the chats is over we will have a Python object representing the paresed HTML, this object acan be used to extract te values int the divs of our intreset,
for example our major intrest in the analysis is the HTML element containing date, time, emojis, gifs, stickers and chats text.
![Chat Preview](https://publicbucketresume.s3.ap-south-1.amazonaws.com/Json.PNG)
- The backend will extract all the necessary data and populate them in various predefined fields to for a json that summarizes the whataspp chats to be use for analysis.
![Chat Preview](https://publicbucketresume.s3.ap-south-1.amazonaws.com/Chat+Contribution.PNG)
- The node backend will relay this json to react fronted, the json thus obtained forms the datasource for various chart js components to render charts giving infographics of the chats
![Chat Preview](https://publicbucketresume.s3.ap-south-1.amazonaws.com/PieChart.PNG)

---

## Features
- Does not store any whatsapp data.
- Runs only on users machine
- Easy to use, user friendly interface
- Give intresting insights and illustrative infographics

---

## Technologies Used
**React.js**   |  **Node.js**   |  **JavaScript.js**  |  **Chart.js**   |   **Python**   |  **Selenium**  |   **Beautiful Soup**   |



## License
>here is the link for my resume [here](https://github.com/IgorAntun/node-chat/blob/master/LICENSE)

