# comp4047-project-1-internet-and-world-wide-web-solved
**TO GET THIS SOLUTION VISIT:** [COMP4047 Project 1-Internet and World Wide Web Solved](https://www.ankitcodinghub.com/product/comp-4047-internet-and-world-wide-web-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;117720&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;2&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (2 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;COMP4047 Project 1-Internet and World Wide Web Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (2 votes)    </div>
    </div>
Group Project: Design and Implementation of a Search Engine

1. Project Specification

In this project, you will design and implement a search engine. This search engine gathers information from the web and then serves users’ requests for searching web contents. In particular, it does not collect information from the web pages listed in a given blacklist (e.g., these web pages contain offensive contents), and it does not record the keywords listed in another given blacklist (e.g., these words are rude or offensive).

1.1 Gathering Information

Write a Java program to gather words in English from HTML documents and their corresponding URLs.

Blacklists: The following two blacklists are given in text file format:

• Blacklist of words: This blacklist contains the words that the search engine would not record and serve (e.g., these words are rude or offensive).

• Blacklist of URLs: This blacklist contains the URLs of the web pages that the search engine would not collect information from (e.g., these web pages contain sensitive or offensive contents). These URLs are expressed in one of the following two forms:

1. Regular form (e.g., http://www.abc.org/index.html).

2. Compact form using the wildcard character “*” (e.g., http://www.abc.org/weapon/* represents all the URLs under the folder named “weapon” in the file hierarchy such as http://www.abc.org/weapon/list.html and http://www.abc.org/weapon/gun/ak37/index.html),

Data structures:

1. URL Pool and Processed URL Pool are used to store URLs, where URL Pool can store at most X URLs (where X is a design parameter; see Step 1 of the following algorithm).

2. Design suitable tables to efficiently store the words and their corresponding URLs.

Algorithm:

1. Input and initialization: The user is prompted to provide: i) a seed URL which serves as a starting point for web search, and ii) the values of the parameters X and Y (where Y is used in Step 4). Assign this URL to URL Pool and set Processed URL Pool to empty.

2. Retrieve and remove a URL from URL Pool on a first-come-first-served basis, add this URL to Processed URL Pool, and get the corresponding web page.

3. Process the web page obtained in Step 2 as follows:

3.1 Extract all words from this web page. For each word, if it is not listed in the given blacklist, store the following items: i) the word, and ii) the URL and the title of the web page.

3.2 Extract the file name (excluding the path and file extension) in src attribute and all words in alt attribute of img tag from the HTML document. For each word, if it is not listed in the given blacklist, store the following items: i) the word, ii) the URL of the web page, and iii) the image URL specified in the src attribute of the image tag.

3.3 Extract all URLs from this web page. For each of these URLs, add it to the URL Pool if it satisfies four conditions: i) it is not listed in the given blacklist, ii) it does not appear in URL Pool, iii) it does not appear in the Processed URL Pool, and iv) the number of URLs in the URL Pool is less than X.

4. If the number of URLs in the Processed URL Pool is less than Y, go to Step 2; otherwise, stop.

1.2 Serving Requests

Write a Java program to serve users’ requests and support the following:

1. Keyword Matching: The user’s query contains a keyword where this keyword can be any word. The program finds the URLs of the web pages which contain the given keyword.

2. Multiple-keywords Matching: The user’s query contains multiple keywords and the logical relationship among these words can only be “AND”, “OR” or “NOT”. A spaces “ ” between two keywords is equivalent to an “AND” operation. The word “OR” between two keywords is equivalent to an “OR” operation. A minus sign “-” just before a word is equivalent to a “NOT” operation.

3. Keyword Matching for image: User can specify to search for images by keywords (either single keyword or multiple-keywords). The program finds the URLs of the web pages that contain images whose file names or alt attributes match the keywords.

The program composes a web page to list the fulfilled URLs with their title. If the user specify to search for images, the fulfilled images will also be displayed in the resulting web page. Then the web server sends this page to the user.

Use Spring (https://spring.io/guides/gs/serving-web-content/), which is a Java web server and framework, for your implementation.

2. Project Information and Announcement

3. Assessment Criteria

1. You must use Java to implement the specification given in Section 1.

2. You are NOT allowed to use any third-party libraries (except the Spring framework mentioned in Section 1) nor database management systems (e.g., MySQL, Oracle, etc.).

3. Design: There are many alternatives to design a search engine. Your design will be assessed in several aspects:

(i) Performance: Is it fast? Is it storage-efficient?

(ii) Program structure: Is it easy to understand, maintain and modify your programs?

4. Implementation: Your implementation will be assessed in three aspects: i) Does it implement all the specified functions? ii) Are there bugs? iii) Is the implementation efficient?

5. Documentation: Your source programs should contain clear and useful comments. Your report should clearly contain sufficient details.

6. Marking scheme:

• Mid-point assessment (10%)

4. Submission and Demonstration

1. Forming Groups

3. Final Submission

• Login into HKBU Moodle.

• Select COMP4047 Project Report

• Upload the file

Email submission is NOT accepted.

3.3 Program and Data Files: Prepare the following files:

• Program files (source files, executable files, etc.).

• Data files which are obtained by executing your search engine with X=10, Y=100 and the following seed URL: https://www.comp.hkbu.edu.hk

The data files contain the gathered words and their corresponding URLs.

• Login into HKBU Moodle

• Select COMP4047 Program and Data Files

• Upload the file

Email submission is NOT accepted.

• If you do not attend this demonstration session, you will be given zero mark for this project.

• During demonstration, we will assess your search engine via a new seed URL, parameters X &amp; Y, blacklist and ignore files.

• During demonstration, you will be requested to compile your program from your submitted source files.
