# FreedomFund

Web scraping application developed by students at UGA for the AADM Freedom Fund.

## Overview of the Project:

Here’s a [link](https://docs.google.com/document/d/1ge8wgcUFPzQh9OQZC-WhiMtNgm_smqViKxc0nHIMH-0/edit) to the project description. Overall, the idea is to build a password protected web application that Athens Anti-Discrimination Movement (AADM) can use internally to identify individuals eligible for their Freedom Fund program.

### Our goal is to:

1. Scrape publicly available data from this [website](http://enigma.athensclarkecounty.com/photo/bookingreport.asp) every morning (on a timer)
1. Process the scraped data into our MongoDB cluster
   - We will have two schema’s: one for user login and storing scraped data
1. Create a Login Page and Home Page
   - Login Page.- We can keep it super basic for now, just email and password
   - Homepage with a form to filter out persons experiencing incarceration from the DB based on certain criteria:
     1. Whether or not they meet the exclusion criteria listed out in the Google Docs linked above
     1. Demographic Characteristics
     1. Agency
1. Backend Using Python Flask
   - Pretty light weight backend frameworks, simpler syntax, and faster deployment

### Technology Stack:

1. Frontend: HTML/CSS and Bootstrap (Responsive Design ftw!)
2. Backend: Python Flask
3. Web Scrape: Python BeautifulSoup
4. Database: SQL - MongoDB

---

## Contributions

In order to push updates to the master branch, a pull request and an approving review from another contributor are required. This avoids conflicts and helps with overall repository organization.

To do this, follow these instructions:

### Create a new branch

```bash
git checkout -b new-branch-name
```

### Stage changes for commit

```bash
git add --all
```

### Commit changes to the branch

```bash
git commit -m "Your commit message"
```

### Push commits to the branch

```bash
git push -u origin new-branch-name
```

### Open a pull request

1.  Go to the [repository](https://github.com/joshmess/AADM-Freedom-Fund) on the GitHub website
2.  Click on the **_Pull requests_** tab
3.  Click the **_New pull request_** button
4.  Set `base` to `master`, and `compare` to `new-branch-name`
5.  Click the **_Create pull request_** button
6.  Leave a comment about what you did, then click **_Create pull request_**

Now wait for another contributor to review and merge it.

### Review a pull request

1.  Go to the [repository](https://github.com/joshmess/AADM-Freedom-Fund) on the GitHub website
2.  Click on the **_Pull requests_** tab
3.  Click on an open pull request
4.  In the first box with a red X, click **_Add your review_**
5.  Click on the **_Review changes_** button
6.  If everything looks good, click **_Approve request_** then **_Submit review_**
7.  Click the **_Merge pull request_** button
8.  Click the **_Confirm merge_** button
9.  Click the **_Delete branch_** button

### Setting Up Dev Environment:

1. Setting up Virtual Environment: virtualenv env
2. Launching Virtual Environment: source env/bin/activate
3. Setting Up Flask: pip3 install flask flask-sqlalchemy flask-login
4. To run the App: Run main.py and open your browswer to http://127.0.0.1:5000/
