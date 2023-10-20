# News-Application

# App Name: GlobalHub

In a news application, sections or categories like _"World," "Business," "Health," "Sports,"_ and _"Tech"_ represent different thematic areas or topics of news content. 

_**Here's a brief description of each section:**_

**World**: The "All" section typically provides a comprehensive overview of news from various categories. It's often the default landing page where users can find a mix of top stories and recent news articles covering a wide range of topics, ensuring users stay informed about a variety of subjects.

**Business**: The "Business" section focuses on news related to the world of business and finance. This may include updates on stock markets, economic trends, corporate developments, entrepreneurship, and financial reports. It's a valuable resource for those interested in the business world and investment.

**Health**: The "Health" section covers news and articles related to health and wellness. This can include medical breakthroughs, health tips, information on diseases and conditions, fitness advice, and updates on healthcare policies and research.

**Sports**: The "Sports" section is dedicated to news about various sports and athletic events. It includes updates on sports leagues, game scores, player profiles, and in-depth analysis of sporting events. It's the go-to place for sports enthusiasts and fans.

**Tech**: The "Tech" section features news on technology and innovation. This may include reports on new gadgets, software developments, startup stories, tech industry trends, and discussions about emerging technologies. It's a valuable resource for tech enthusiasts and professionals.

Each of these sections caters to a specific audience or interest group and provides news and information relevant to those topics. News applications often organize content in this way to help users find and explore articles and updates that align with their interests.

The app's each page's screen shot is added at the end.

_**Process on how to run the app:**_

In cmd, migrate to News-Application folder created. 

Using the command 'npx expo start', start the metro bundler. As I have Expo go installed in my android app, scan the QR from the app. 

Once your homepage appears, enter the login credentials and login. Here I've used Admin and Password as Username and Password.

At the bottom of the phone screen, we have 5 sections. Select any one of the section and view the news headlines.




Screenshots:

Login Page:

![IMG-20231020-WA0019](https://github.com/soumyapandit0415/News-Application/assets/91374416/084be733-9e56-47f5-849e-23ccff38da4c)

World News:

![IMG-20231020-WA0020](https://github.com/soumyapandit0415/News-Application/assets/91374416/a3f601c7-0fd5-4d3b-8b47-22e8d4abc770)
![IMG-20231020-WA0021](https://github.com/soumyapandit0415/News-Application/assets/91374416/be61c41e-b3cc-4f1a-8e47-a72a34a52965)

Business News:

![IMG-20231020-WA0022](https://github.com/soumyapandit0415/News-Application/assets/91374416/beb782c8-a8ff-428b-845b-ae7977db53da)
![IMG-20231020-WA0023](https://github.com/soumyapandit0415/News-Application/assets/91374416/d15ab7cf-1f5d-4141-b990-5dee9431322e)

Health News:

![IMG-20231020-WA0024](https://github.com/soumyapandit0415/News-Application/assets/91374416/1e88ba32-2813-4499-b82f-3b2f60c6c1f4)
![IMG-20231020-WA0025](https://github.com/soumyapandit0415/News-Application/assets/91374416/4ae17e5d-0c38-445d-8b22-ca42b85ddf6b)

Sports News:

![IMG-20231020-WA0026](https://github.com/soumyapandit0415/News-Application/assets/91374416/d1e0a82b-1eb3-4b80-b5b6-23f11b01dc52)
![IMG-20231020-WA0027](https://github.com/soumyapandit0415/News-Application/assets/91374416/b5a1d2e2-ee61-42d6-bfe9-f69f00007904)

Tech News:

![IMG-20231020-WA0028](https://github.com/soumyapandit0415/News-Application/assets/91374416/ca194d95-c662-45ee-85eb-4a0e7d744d84)

As there aren't any tech news available, the app keeps bufferning until it gets tech related news from API.

**Data Structure:**

**newsData (useState)**: Data is fetched from an external source using the services('general') function and stored in the newsData state variable. It represents an array of news articles.

**FlatList (from NativeBaseProvider):** The FlatList component is used to render and display a list of news articles. It takes the newsData array as its data source.

**JavaScript Objects (item):** The individual news articles are represented as JavaScript objects with properties like title, publishedAt, description, and urlToImage. These objects are part of the newsData array.

**Styles (styles object):** The styles object is used to define various styles for elements in the UI, including the news container, title, description, date, and spinner.

**Constants (grey, yellow):** The grey and yellow constants store RGB color values used for styling various components in the UI.

The useEffect hook is used to fetch news data when the component mounts, and the data is subsequently displayed using the FlatList component. If there is no data yet (i.e., newsData is empty), a spinner is displayed to indicate that the data is being loaded.

Overall, the code primarily relies on arrays and objects to represent and manage news data and uses style objects for UI styling. It also utilizes components provided by NativeBase for UI rendering and styling.

