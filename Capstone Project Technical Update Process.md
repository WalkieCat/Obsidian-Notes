## Feature 1: Share button disappearing bug fix 
**What it is**:
On the result page for a survey, when the user click on the "Share" button and escape the share box, the "Share" button disappear completely. The button does not render and only rendered after the website was reloaded.

**What the problem was**:
The entire "Share" block was removed under a function called `elementsToRemove` , which deleted anything under a class called `non-rendered` and `headerprint` . If the user clicked outside of the 
"Share" region without completing the process, the elements get deleted and never got reloaded back in.

**What the fix was**:
Instead of using `elementsToRemove` the function was renamed into `elementsToHide` . This function adds the elements into a temporary state of being hidden for the process, which gets displayed if the user ends the process without completing it, or completes the process.


## Feature 2: Download survey results PDF with personal information of the user
**What it is**:
The current implementation of the PDF download function downloads the result of certain survey, it only downloads the survey results. The sponsor requested the PDF survey result to includes personal information - full name, age and gender within the PDF.


**What the implementation was**:
Modified the download function to includes the personal information. This was achieved by appending the user information briefly on the results page. This information will then be appended into the PDF and deleted immediately. The PDF dimension is modified to include this information block on the top.

## Feature 3: Updating the survey dashboard
**What it was:**
The sponsor requested new surveys to be added from their new book, along with new survey logos. The new surveys are to reflect their new understanding of the physical fitness booklet.

**What the feature was:**
Following the new booklet received from the sponsor, the team updated the new surveys into the webpage.

## Feature 4: Moved the email from server side to client side
**What it is and the problem:**
The current email sharing request was conducted through Google's `smtp.gmail.com` using a Gmail account. This account will try to authenticate using it's credential to send the email using that address. However, this account either does not exist or has its credential changed. This feature has not worked through manual testing of the credentials. 

**What the fix was:**
The entire emailing feature has been moved to the client side. How this works:
- When the user clicks on the 'Share' button, a window will pop up asking if the user wants to use Outlook or Gmail
- The survey result will be downloaded and an email template will be opened in the user's mailing service 
- The template will remind the user to attach the survey into the email and remove template text before sending

This was verified manually and has been confirmed as working. A mailing service was considered but was decided to be out of scope, due to the complexity and time constraint presented by the alternative option.

## Feature 5: New homepage update with booklet
**What it was:**
The sponsor requested a new homepage completed with a brief description about the mission of the website and the updated booklet.


**What the new feature was:**
A new homepage was designed with the description of the website taken from the booklet that was received from the sponsor, and a link to the booklet was included on the website to download the booklet.

## Feature 6: New logos and website formatting
**What it was:**
New logos for the survey was implemented, styling designs were made to improve the overall look of the website. The main function of the feature was to made the website easier to navigate, more aesthetically pleasing, and make UI elements easier to find. Subsequently, a new survey called `howAreYouGoingSurveys.js` was added at this stage, but has not been fully populated with survey questions. 

## Feature 7: Added new surveys and started data collection
**What it was:**
The sponsor requested the addition of two new surveys `20mRun` and `elite20mRun` to be added onto the surveys page. `20mRun` was reserved for regular folks and students, while `elite20mRun` was reserved for professional athletes. Survey questions have been updated to match the questions present in the booklet, along with question numbers for tracking purpose.

**What the implement was:**
After some internal documenting of file naming convention, it was discovered that `20mRun` and `elite20mRun` did not follow the standard file naming convention for surveys. These files were renamed to `run20mSurveys.js` and `elite20mRunSurveys.js` . These files were then passed into `collection_name` in `dashboard.vue` to start a collection process for the survey data. `results.vue` was also updated to display the results from `run20mSurveys.js` and `elite20mRunSurveys.js` . For this collection to work, `firebase.js` was changed to include a new collection and exported under the same name. 

At the same time, the function `camelCaseToSentenceCase` present inside `helpers.js` was identified to have an issue with the naming convention, where it would only slice the survey name at a capitalized letter and not numbers. This was changed to include name slicing at numbers, ensuring all survey appears with the same styling.

A majority of existing tests were updated, with some identified as redundant and combined with existing test. 

## Feature 8: Mostly UI fixes
**What it was:**
This section features further UI fixes such as spelling correction, formatting of the survey results page and rearranging surveys to match the order that they are in within the booklet. 



## Jian's Change notes:

**Feature 7.1?: Updated survey questions**
To ensure all relevant questions match those from the booklet, every test had been reviewed and updated. All relevant tests that have been reviewed also have the questions number included as a comment to make easier to track. Majority of existing tests were updated, but some tests have been made redundant and combined with existing test, *which are still present in the folder for future reference (we should decide either to keep them and rename them as 'old' tests or delete them) 

**Feature 8 (maybe 6?): results page reformatting**
The formatting of the results page was updated to improve result visibility. 

The design of the existing results page used box containers for each survey to display results if they exist. The page rendered every box even if there are no results for a particular survey, and the small size of the boxes made the visibility of these results fairly difficult to identify from a glance. 

The change made the page only display the latest results of completed surveys, hiding surveys with no results. Surveys with multiple historical results has a 'view history' button which shows a (modal) pop-up window with historical results. These changes reduces clutter on screen and allows users to focus on one object at a time while viewing. 

this is a test change made from obsidian itself