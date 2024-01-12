# mojposao_web_scraping

Goal was to pull basic information about job listings such as workplace title, employer, location and end date to apply for the job.

Starting off with the required libraries, Python version 3.11.5, BeautifulSoup version 4, Pandas version 2.1.4 and requests installed in miniconda3. Loaded URL shows results for jobs in IT and telecommunications role. 
Search for the needed information began with recognising the id containing all that we want to import into our dataframe, in this case it was "featured-jobs". After that a FOR loop was initiated to pull all elements per job 
listing.  Since the employer name was contained in an image section, it was a two-step process to acquire the "title" information. All information was then loaded into a dictionary, afterwards into a new dataframe and 
finally  into our original dataframe. When the loop ended, upon viewing the dataframe I've noticed the  "\n" in the Title column so an additional line was required to clean up the table further. Information was loaded into a 
regular .csv file which is avaliable for viewing in the repository.

