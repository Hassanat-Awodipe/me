# How to Add A Table of Content (TOC) to your Jupyter Notebook

![image](https://user-images.githubusercontent.com/45914807/188284741-206b1c75-c69a-4bad-a86d-01d73824ae80.png)

> I did not know table of content could be added to a Jupyter Notebook unitl I started the Udacity Nanodegree and had to do some projects. The second project turned out to be a really long notebook so, my reviewer suggested I added a TOC.
>
> The previous project had a TOC so I just copied, pasted and edited accordingly but there was a limitation; my current project had several sub-sections. The TOC was designed such that the link to the section was embedded in the section name. For example, if you clicked `Conclusion`, it would take you directly to `Conclusion`. When I tried this with the `copy and paste template`, the links in the sub-sections redirected to the main section. That method only worked for the main topics.
> 
> Here is what I did: I had to learn a bit of html, at least the amount useful for Markdown cells. I will explain this using the first section in the image above which was taken from my Jupyter noebook.
> 
> * The `<a></a>` tag defines a **hyperlink**
> * href="#Data-Gathering" refers to the link destination. It is an **attribute** of the `a` tag 
> * `Data Gathering` is what you get to see i.e the statement in which the link is embedded or the **link text**.
>        
> You may check the image to understand the hyperlink and link text better 
  
```
# Table of Content

1. <a href="#Data-Gathering">Data Gathering</a>   
1\.1\. <a href="#From-a-CSV-File">From a CSV File</a>  
1\.2\. <a href="#From-an-Internet-File">From an Internet File</a>  
1\.3\. <a href="#Query-Twitter-API">Query Twitter API</a>  

2. <a href="#Assessing-Data">Assessing Data</a>  
2\.1\. <a href="#WeRateDogs-Archive">WeRateDogs Archive</a>  
2\.2\. <a href="#Image-Predictions">Image Predictions</a>  
2\.3\. <a href="#Tweet-API-Data">Tweet API Data</a>  
2\.4\. <a href="#Quality-Issues">Quality Issues</a>  
2\.5\. <a href="#Tidiness-Issues">Tidiness Issues</a>     

3. <a href="#Cleaning-Data">Cleaning Data</a>  
3\.1\. <a href="#WeRateDogs_clean">WeRateDogs_clean</a>  
3\.2\. <a href="#Image_predictions">Image_predictions_clean</a>  

4. <a href="#Storing-Data">Storing Data</a>  

5. <a href="#Analyzing-and-Visualizing-Data">Analyzing and Visualizing Data</a>  
5\.1\. <a href="#Analysis-Questions:">Analysis Questions</a>  
5\.1\.1\. <a href="#1.-Which-dog-stage-had-the-number-of-highest-rating?">Question 1</a>  
5\.1\.2\. <a href="#2.-How-has-the-interactions-on-WeRateDog-improved-over-the-years-the-data-was-collected?">Question 2</a>  
5\.1\.3\. <a href="#3.-What-breed-of-dog-is-mostly-interacted-with-by-WeRateDog-followers-based-on-retweet-and-favourite-count?">Question 3</a>  
5\.1\.4\. <a href="#4.-Do-you-think-the-followers-agree-with-the-ratings?">Question 4</a>  
5\.2\. <a href="#Insights:">Insights</a>  
5\.3\. <a href="#Visualizations">Visualizations</a>  
```

> The codes looks straightforward, right? But this is the trick:

```
## Data Gathering
<a id="optparam"></a>
```

```
#### 1. From a CSV file
<a name="From-a-CSV-File"></a>
```

> The attributes for the main section and the sub-section are different. 
> 
> While the main section (data gathering) used `<a id="optparam"></a>`, the sub-section (From a CSV File) used `<a name="sub-section-name"></a>` and it included the name of the subsection. Spaces in the link destination are reprsented with (-). 
> 
> The tag, attribute and link destination for all the main sections were the same but not the sub-sections. The difference was with the name of the sub section


---

Side Note: I also learnt that you could add two space bar at the end of your cuurent line to take the cursor to the next line.






