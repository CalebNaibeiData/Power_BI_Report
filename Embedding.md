# How to Publishing and Embedding Power BI Reports on the Web with IFrames

## Introduction

After a succesfull cleaning, analysing and making of report in Power BI, the next step to some Users Is to Embed it to a website or a blog.
In this guide I will walk you through how I :
* Created working space in Power BI.
* Upload and Published Report
* Generate and Embeded Code With IFrame

> IFrames involves generating a shareable link or code from the Power BI service and placing that code into the HTML of your website.


<img width="1354" height="667" alt="Screenshot 2026-04-06 033011" src="https://github.com/user-attachments/assets/ef30786c-b7fa-4036-9adc-b8906493c05f" />

*This was my Dashboad*

---

## Step 1: Creating a Workspace in Power BI Service

> A workspace is used to store and manage reports, dashboards, and datasets.

### Follow these steps:
1. Go to Power BI Service: https://app.powerbi.com
2. Sign in with your account
3. From the left panel, select **Workspaces**
4. Click **New Workspace**
5. Enter a name (e.g., *Electronics Sales Workspace*)
Click **Save**


![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/4nmxikoudjwvtoe1auu8.png)

---

## Step 2: Upload and Publish the Report
After the workspace is created, upload your Power BI report file.

### Steps On Power BI:

1. Click **Publish**
2. Select your **workspace**


![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/6kmd7a6ar2mnn7jg3ijq.png)

---

## Step 3: Understand Embedding Options
Power BI provides two main ways to embed reports:

### 1. Publish to Web (Public Embed)

- Accessible without login
- Suitable for public dashboards
- Generates a public link

### 2. Secure Embed

- Requires authentication
- Suitable for private or organizational use
- Keeps data protected

If “Publish to Web” is disabled, use Secure Embed.

> After Selecting The Prefered one You Proceed to embed the report, generate an iframe code from Power BI.

### Steps:

1. Open your report in Power BI Service
2. Click **File** then **Embed report** then **Website or portal**
3. Copy the generated IFrame code



![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/vcb5jh8g9ovh3spu1hyg.png)

---

## Step 4: Embed the Report in an HTML Page

Create an HTML file and paste the embed code inside it.


![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/17azstt40gypz4o0zwh7.png)*HTML page displaying the dashboard*

---

## Here are Common Issues You Might Come Accross and Solutions

### Issue 1: Report Not Displaying

- Cause: Using a secure embed link without authentication
- Solution: Log in or use “Publish to Web” if available

---
### Issue 2: Map Visual Not Working
Cause: Map visuals disabled in settings
Solution:

- Go to **File** then **Options** then **Global** then **Security**
- Enable map visuals

---
### Issue 3: Incorrect Calculations

- Cause: Improper DAX or data modeling
- Solution: Use row-level calculations

---
### Issue 4: Slicers Not Working

- Cause: Using fields from the fact table
- Solution: Use dimension tables (e.g., Customers, Products)

--- 
## Best Practices

1. Use a star schema for data modeling
2. Create measures using DAX instead of raw columns
3. Use consistent naming for visuals
4. Keep the dashboard layout clean and aligned
5. Use slicers from dimension tables only

---

## Conclusion

Power BI reports Can Be Published and Embeded in Websites using IFrame while following the above steps.

Understanding all the stapes and possible solutions for issues that you might come accross Helps in Smooth Implementation.
Here was the initial raw data[electronics sales data (1).xlsx](https://github.com/user-attachments/files/26492231/electronics.sales.data.1.xlsx)
