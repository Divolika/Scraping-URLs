# Scraping-URLs

This assignment involved creating a Python program to automate web scraping from Google search results. The goal was to perform a Google search for a specified query, extract URLs from the search results, visit each URL, and scrape relevant data from those web pages. Here’s a breakdown of the key steps and tools used:

1. **Performing Google Search:** 
   - We constructed a Google search URL using the input query and sent a GET request to retrieve the search results page.
   - The response content was parsed using BeautifulSoup to locate and extract all the search result links.

2. **Extracting URLs:**
   - From the parsed search results, URLs were extracted by filtering out irrelevant links and retaining those that started with '/url?q='.
   - These URLs were then cleaned and prepared for subsequent scraping.

3. **Scraping Individual Pages:**
   - For each URL, a GET request was sent to fetch the page content.
   - BeautifulSoup was used again to parse the HTML and extract specific data: the page title and the textual content of paragraphs.

4. **Storing Results:**
   - The scraped data, including titles and paragraph text, was compiled into a document format.
   - The final results were saved into a text file, providing a consolidated view of the scraped information.

5. **Downloading the Document:**
   - The resulting text file was made available for download, ensuring easy access to the compiled data.

This assignment provided practical experience with web scraping, demonstrating the use of Python libraries like Requests and BeautifulSoup for data extraction from web pages. By automating the scraping process, we were able to efficiently gather and process information from multiple web sources, showcasing the potential for such techniques in data analysis and research applications.
