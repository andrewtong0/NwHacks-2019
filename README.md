# ProfStats

![Sample Output of a ProfStats Query](https://i.imgur.com/Med1pYx.png)

ProfStats was my team's submission to the nwHacks 2019 Hackathon. You can find our full submission details at our devpost link, [here](https://devpost.com/software/profstats) Our project was a nominee for Microsoft's "Azure Prize Champ", and Hootsuite's "Hack that Best Champions the Power of Human Connection".

### How It Works
- The user queries a professor to a Slack bot
- The bot communicates with our database to check whether the professor's data already exists there - if not, it webscrabes with BeautifulSoup and Selenium to gather data from various sites (e.g. RateMyProfessor, SlackNotes, etc.)
- After gathering data, presents it in an image format back to the user

### Dependencies
- Slack (requires authentication token and account to use)
- BeautifulSoup4 and Selenium + Chrome Webdriver (for web scraping)

### Time Restraints
Due to time restrictions, we were unable to fully implement everything we wanted to. Slated additions that we were unable to accomplish include:
- Implementation as a Chrome Extension with automatic professor identification (e.g. when a student views a course on the UBC website, the extension would create an automatic popup of the professor)
- Further database implementation and optimization, as the current version has minimal interaction and utilization of it
- Additional machine learning with Azure to parse user reviews to refine professor ratings as a mixture of RateMyProfessor data as well as other gathered data interpreted with ML
- Hosting data on API endpoints with Standard Library for quicker and easier access
- Creation of radar graphs coupled with professor attribute data to give students another quick way to interpret professor strengths/weaknesses

### Project Notes
- Project was created during the hackathon time period of 24 hours on January 26-27, 2019
- Team consisted of four people; Brandon Chung, Christopher Hui, Shirley Bi, and myself
- Original unforked repository can be found [here](https://github.com/bchung00/NwHacks-2019)
